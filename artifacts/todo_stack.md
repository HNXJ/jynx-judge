# todo stack

Top = next. Gate: `PYTHONPATH=src python -m pytest tests -q`.

- T-1 Add a dev requirements file with `pytest` and `pytest-asyncio`; `tests/test_game_controls.py::test_game_controller_dry_run_turn_is_truth_safe` is async and fails with "async def functions are not natively supported". Closes when: after installing it, `PYTHONPATH=src python -m pytest tests -q` reports 0 failed. Blocked by: none.
- T-2 Rename package `src/gamma_labyrinth` and `src/run_gamma_labyrinth.py` to the repo name, imports and tests included. Closes when: `git grep -n gamma_labyrinth -- src tests` prints nothing and the gate reports 0 failed. Blocked by: T-1.
- T-3 Triage open issues #1 to #5. Closes when: `gh issue list -R HNXJ/jynx-judge --state open --json number -q length` prints 0. Blocked by: none.
