# Zenith Mesh Lease Mesh Walkthrough

This walk-through keeps the domain vocabulary close to the data instead of burying it in prose.

| Case | Focus | Score | Lane |
| --- | --- | ---: | --- |
| baseline | quorum health | 153 | ship |
| stress | lease drift | 154 | ship |
| edge | replica lag | 180 | ship |
| recovery | membership churn | 179 | ship |
| stale | quorum health | 227 | ship |

Start with `stale` and `baseline`. They create the widest contrast in this repository's fixture set, which makes them better review anchors than the middle cases.

The next useful expansion would be a malformed fixture around lease drift and membership churn.
