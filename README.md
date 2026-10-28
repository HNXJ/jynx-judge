# gamma-labyrinth

Pluggable validators and rubrics with typed outcomes.

Proposed future name: **jynx-judge** (proposal, not renamed yet)

## Place in the 7-repo layout

Plane: **JUDGE**. See [HNXJ/jynx-arena](https://github.com/HNXJ/jynx-arena) and its [architecture](https://github.com/HNXJ/jynx-arena/blob/main/docs/protocol/ARCHITECTURE.md) (ARENA, RULES, SCIENCE, LAB, ENGINE, JUDGE, WORLD). The current jynx-arena runtime is proposed to become **jynx-engine**; **jynx-world** (event ledger, projections) is a new proposed repo.

## Holds today

- `src/gamma_labyrinth/` including `judge.py` (TrophyJudge) and game/server code, with `tests/`.
- Doctrine in `docs/doctrine/`; `events/`, `runtime/windows/`, run scripts.
- World-seed material here is proposed to move to the new **jynx-world**.

## Shared root layout (target, not yet applied)

`artifacts/`, `docs/`, `src/`, `schemas/`, `tests/`, `tournaments/`, `README.md` — see [SHARED_ROOT_LAYOUT](https://github.com/HNXJ/jynx-arena/blob/main/docs/protocol/SHARED_ROOT_LAYOUT.md).

## Truth safety

A Judge PASS means a submission met a rubric under a protocol version; it is not scientific truth.

