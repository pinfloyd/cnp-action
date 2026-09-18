# AI Admissibility Action — compatibility surface

This repository keeps the historical workflow slug `pinfloyd/cnp-action` available for compatibility with existing references.

It is **not** the canonical repository for new public evaluation installs.

For new evaluations, use:

https://github.com/pinfloyd/ai-admissibility-action

Official public demonstration surface:

https://ai-admissibility.com/

## Current implementation status

The composite Action in this repository performs fail-closed preflight validation but **does not call a runtime authority**. After successful preflight it intentionally stops with:

`FAIL_CLOSED: runtime authority integration is not wired yet`

That behavior is deliberate. This repository must not be interpreted as a working production authority integration.

Historical direct-runtime self-test workflows that expected an open public `/pubkey` or direct public ALLOW/DENY access have been retired from `main`. The active public runtime check is the bounded `verify-public-boundary-contract-v2` workflow.

## What it demonstrates

- required admission inputs are checked;
- placeholder or incomplete values are rejected;
- a non-PASS trust verdict is rejected;
- execution does not silently continue when runtime authority integration is absent.

## What it does not claim

- no live production authority integration;
- no customer-specific no-bypass guarantee;
- no self-serve production access;
- no payment or credential-issuance path;
- no scanner or post-hoc monitoring capability.

## Public role

The website and GitHub repositories are showcase, documentation, proof, and demonstration surfaces only. They are not used as commercial customer runtime infrastructure.

- Product / demonstration site: https://ai-admissibility.com/
- Current Marketplace evaluation Action: https://github.com/pinfloyd/ai-admissibility-action
- Boundary architecture / proof: https://github.com/pinfloyd/ai-admissibility-boundary
- Collaboration: governance@ai-admissibility.com

**No Admission = No Execution.**
