# Ramanujan–Petersson

This repository contains the source note and a Gauss-managed Lean formalization companion for the
Ramanujan–Petersson argument recorded in `ramanujan-petersson.md`.

## Layout

- `ramanujan-petersson.md`: source Markdown
- `ramanujan-petersson.pdf`: source PDF
- `lean/`: Lean 4 project
- `lean/README.md`: public statement of the current formalization boundary

## Lean Companion

The Lean project exposes a paper-facing public layer for the main statements together with
supporting companion documents:

- `lean/blueprint.md`
- `lean/claims.yaml`

The private review queue `paper_patch.md` is intentionally not included in this public snapshot.

## Build

```bash
cd lean
lake update
lake build
```

The exported project is pinned to `leanprover/lean4:v4.26.0` and references `mathlib4` by git
revision so that the public snapshot can be built outside the private research environment.
