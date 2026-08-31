# Triad-Test

**Triad-Test is the independent executable validation organization for triadic admissibility.**

It tests how multiple admissibility dimensions combine at a consequence boundary, including GCAT/BCAT, ECAT/ICAT, recoverability, and conservative admissible-existence conditions.

## What belongs here

- **tests** — executable triadic gate, fixtures, receipts, and regression cases;
- **Documentation** — mathematical assumptions, test parameters, and interpretation guidance.

## Core test shape

A candidate consequence is evaluated across the required dimensions and produces an explicit result such as:

```text
ALLOW
DENY
FAIL_CLOSED
```

The test harness is intended to expose composition failures, missing basis, stale or contradictory evidence, and cases where strong local results do not justify a composite consequence.

## Boundary

A passing test demonstrates only that the frozen case satisfied its declared predicates. It does not create execution authority, prove an untested theorem, or promote another repository or runtime into an activated state.
