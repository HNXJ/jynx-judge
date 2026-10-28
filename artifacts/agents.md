# agents

Independent verification: judges that score submissions against a rubric.

## Layout

- `src/gamma_labyrinth/` judge package (`judge.py`, `controls.py`, `server.py`, `core/types.py`); `src/run_gamma_labyrinth.py` entry.
- `tests/` pytest. `docs/doctrine/` reference. `schemas/`, `tournaments/` empty. `artifacts/archive/` retired files.

## Build and test

```
python -m venv .venv && .venv/bin/pip install pytest pytest-asyncio
PYTHONPATH=src .venv/bin/python -m pytest tests -q
```

Gate: the command above; read its summary line. Root layout check (needs a jynx-engine checkout): `python <jynx-engine>/src/scripts/check_shared_root.py .` prints `OK`.

## Git

- Work on `_temp_<name>` branches; PR to `main`. No direct push to `main`.
- Stage exact paths; never `git add .` or `-A`.
- Never commit `.env`, tokens or keys.
