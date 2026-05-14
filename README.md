# cnp-action

**Fail-closed admission gate for GitHub Actions**

`cnp-action` is the public GitHub Action surface for AI Admissibility / controlled negotiation protocol (CNP) evaluation.
It is designed to stop execution when required admission context is missing, invalid, or incomplete.

## What it is

- A fail-closed gate for GitHub automation.
- A public Action-facing surface for external admission evaluation.
- A way to make one thing clear fast: execution must not continue on missing admission context.

## What it is not

- Not a scanner.
- Not a post-hoc reporting layer.
- Not a generic security toolbox.
- Not a self-authorizing policy loop.

## What it does

- Checks for required admission inputs.
- Rejects incomplete or invalid runtime context.
- Fails closed instead of silently continuing.

## Example usage

```yaml
jobs:
  admission-check:
    runs-on: ubuntu-latest
    steps:
      - uses: pinfloyd/cnp-action@v0.1.1
        with:
          authority-url: https://example-authority.company.tld/admit
          authority-pubkey: sha256:replace-with-pinned-authority-pubkey
          policy-id: ai-secrets-v1
          trust-verdict: PASS
```

## Input meaning

- `authority-url` - external authority endpoint URL.
- `authority-pubkey` - pinned authority public key or pinned authority identity value used by the caller.
- `policy-id` - policy identifier expected by the admission flow.
- `trust-verdict` - runtime trust verdict; must be `PASS` for the Action to proceed beyond preflight checks.

## Commercial route

For real commercial use above the public GitHub surface, use the canonical inquiry entry:

[Request access](https://ai-admissibility.com/request)

GitHub is not checkout.
The public Action surface is an evaluation / understanding path, not the commercial fulfillment path.

## Core message

Pre-run policy is necessary. External admission is the stronger boundary.

Platform-native controls improve the executor. External admission separates execution from authority.

If execution can proceed without an external allow decision, the system has policy, but not external admission authority.

**No Admission = No Execution.**

Learn more:
- https://ai-admissibility.com/platform-native-policy/
- https://ai-admissibility.com/external-admission-authority/
- https://ai-admissibility.com/surrogate-boundary-test/
