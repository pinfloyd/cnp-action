# Roadmap

## Current proven stage

This public repository is a compatibility surface, not the canonical runtime.

Current proven properties include:

- deterministic fail-closed preflight behavior;
- compatibility for the historical `pinfloyd/cnp-action` slug;
- public documentation and examples;
- an active public boundary-contract regression workflow;
- explicit separation between this Action and the canonical installed boundary.

## Current maintenance direction

The repository should remain small and unambiguous:

- preserve compatibility for existing references;
- keep fail-closed behavior intact;
- keep the public regression workflow aligned with `proof-status.json`;
- avoid reintroducing public checkout, payment, credential issuance, or hosted-runtime claims;
- point new evaluation users to `pinfloyd/ai-admissibility-action`;
- point canonical live demonstration traffic to https://ai-admissibility.com/canonical-pilot/.

## Historical material

Older release and workflow history may refer to private self-tests, direct public authority probing, or Hosted Authority assumptions from earlier product stages.

Those are historical artifacts, not current public runtime claims.

## Not claimed

This roadmap does not claim:

- live production authority integration in this Action;
- customer-specific no-bypass protection;
- public production access;
- public checkout or credential issuance.

**No Admission = No Execution.**
