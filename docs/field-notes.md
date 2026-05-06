# Field Notes

This note keeps the distributed systems assumptions visible beside the checks.

The domain cases cover `quorum health`, `lease drift`, `replica lag`, and `membership churn`. They sit beside the smaller starter fixture so the project has both a compact scoring check and a domain-flavored review check.

`stale` tells me the happy path still works. `baseline` tells me whether the guardrail still has teeth.

The language-specific addition keeps the review model as queryable sqlite views and assertions.
