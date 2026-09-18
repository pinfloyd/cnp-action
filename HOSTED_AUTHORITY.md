# Hosted Authority — historical/reference note

## Current status

This repository is the compatibility Action surface for older references to `pinfloyd/cnp-action`.

It is **not** the canonical installed runtime, not a public production authority, not a checkout surface, and not a credential issuer.

The current public product and demonstration surface is:

https://ai-admissibility.com/

The current canonical live demonstration uses the installed boundary identity:

`AI_BOUNDARY_RELEASE_V1`

## Repository role

This repository currently provides:

- compatibility for the historical Action slug;
- deterministic fail-closed preflight behavior;
- public documentation and examples;
- the public boundary-contract regression workflow.

Runtime authority integration is not wired in this Action.

## Historical Hosted Authority material

Older versions of this repository described a Hosted Authority commercial path and public runtime assumptions that no longer represent the current public product surface.

Those earlier concepts remain part of repository history and published tags. They are not rewritten.

## Current collaboration path

The website and GitHub repositories are showcase, documentation, proof, and demonstration surfaces.

For research, integration, collaboration, or deployment discussions:

**governance@ai-admissibility.com**

No public checkout, payment, automatic credential issuance, or customer production runtime is provided by this repository.

## Current verification

The active public regression contract is:

`.github/workflows/verify-public-boundary-contract.yml`

It verifies the published proof-status contract, protected public identity endpoint, rejected anonymous admission, and canonical public routes.

**No Admission = No Execution.**
