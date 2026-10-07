# Proposed roadmap

## M1 — Taxonomy and specification

- Publish the fixture taxonomy and expected-result schema.
- Define observable, Maven-resolved and unresolved/conflicting fact classes.
- Fix acceptance tests and adapter boundaries.

## M2 — Fixture corpus

- Publish at least 20 deterministic synthetic fixtures.
- Produce fixed hashes and documented expected observations.
- Validate redistribution and per-file licensing.

## M3 — Java conformance harness

- Implement the Java 17 CLI and JUnit integration.
- Run fixtures deterministically and retain raw tool outputs.
- Support bounded, offline repeat execution after tool setup.

## M4 — Tool adapters and reports

- Add at least three adapters selected after compatibility checks.
- Produce JSON and human-readable reports.
- Document unsupported assertions instead of treating them as failures.

## M5 — Public release

- Add CI examples and contributor guidance.
- Report reproducible findings upstream, with patches where feasible.
- Publish a tagged release and limitations statement.

