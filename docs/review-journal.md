# Review Journal

This journal records the domain cases that matter before widening the public API.

The local checks classify each case as `ship`, `watch`, or `hold`. That gives the project a small review vocabulary that matches its distributed systems focus without claiming live deployment or external usage.

## Cases

- `baseline`: `quorum health`, score 153, lane `ship`
- `stress`: `lease drift`, score 154, lane `ship`
- `edge`: `replica lag`, score 180, lane `ship`
- `recovery`: `membership churn`, score 179, lane `ship`
- `stale`: `quorum health`, score 227, lane `ship`

## Note

The repository should be understandable without pretending it is larger than it is.
