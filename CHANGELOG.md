# Changelog

## Current surface state

The current `main` branch is a public compatibility and evaluation surface.

Current state includes:

- README language aligned to showcase / evaluation semantics;
- deterministic preflight fail-closed Action behavior;
- public boundary-contract verification against the canonical site;
- removal of obsolete manual workflows that expected an open public pubkey endpoint or direct public ALLOW/DENY authority access.

## Historical releases and runs

Older tags, commits, and workflow runs are retained as historical evidence.

They may contain terms or assumptions from earlier stages, including:

- private repository language;
- Hosted Authority commercial-path language;
- direct `/pubkey` probing that expected HTTP 200;
- direct public `/admit` ALLOW/DENY tests.

Those historical objects are not rewritten and do not supersede the current public contract.

## Current public contract

Current public semantics are:

- canonical live demonstration: https://ai-admissibility.com/canonical-pilot/
- public identity endpoint: intentionally protected;
- anonymous admission: intentionally rejected;
- Marketplace / Action surfaces: evaluation only;
- customer production no-bypass: not claimed by this repository.

**No Admission = No Execution.**
