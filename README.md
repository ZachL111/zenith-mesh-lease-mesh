# zenith-mesh-lease-mesh

`zenith-mesh-lease-mesh` is a SQL project in distributed systems. Its focus is to implement an SQL distributed systems project for lease state machine modeling, using transition tables and invalid-transition tests.

## Why It Exists

I want this repository to be useful as a quick reading exercise: fixtures first, implementation second, verifier last.

## Zenith Mesh Lease Mesh Review Notes

The first comparison I would make is `quorum health` against `quorum health` because it shows where the rule is most opinionated.

## Features

- `fixtures/domain_review.csv` adds cases for quorum health and lease drift.
- `metadata/domain-review.json` records the same cases in structured form.
- `config/review-profile.json` captures the read order and the two review questions.
- `examples/zenith-mesh-lease-walkthrough.md` walks through the case spread.
- The SQL code includes a review path for `quorum health` and `quorum health`.
- `docs/field-notes.md` explains the strongest and weakest cases.

## Architecture Notes

The repository has two validation layers: the original compact policy fixture and the domain review fixture. They are separate so one can change without hiding failures in the other.

The SQL checks add a separate view over the domain review fixture.

## Usage

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File scripts/verify.ps1
```

## Tests

The same command runs the local verification path. The highest-scoring domain case is `stale` at 227, which lands in `ship`. The most cautious case is `baseline` at 153, which lands in `ship`.

## Limitations And Roadmap

The fixture set is small enough to audit by hand. The next useful expansion is malformed input coverage, not extra surface area.
