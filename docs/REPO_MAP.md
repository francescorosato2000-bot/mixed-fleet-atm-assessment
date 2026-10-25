# REPO_MAP

Map of the files and folders of this repository, so that an AI assistant does not have to scan the tree.
Update this file whenever you add, move or delete something. Status: **exists** or **planned** (created later, see `docs/project/REPO_BLUEPRINT.md`).

## Inside the repo (`TUD\mixed-fleet-atm-assessment`)

| Path | Purpose | Tracked by Git | Status |
|------|---------|----------------|--------|
| `README.md` | Public front page (to be rewritten near the end) | yes | exists |
| `.gitignore` | Files Git must ignore | yes | exists |
| `requirements.txt` | Pinned Python environment (Python 3.12, BlueSky 1.1.1) | yes | exists |
| `docs/REPO_MAP.md` | This file | yes | exists |
| `docs/project/` | **Private** planning files | **no** (ignored) | exists |
| `docs/bluesky_notes.md` | Learning log on BlueSky: verified commands, formats, defaults, each with its source and the test that confirmed it | yes | planned |
| `docs/bluesky_wiki_index.md` | Our index of the ~15 wiki pages that matter, grouped by topic, with file names | yes | planned |
| `docs/assumptions.md`, `docs/metrics.md`, `docs/performance_model.md` | Assumptions, metric definitions, physics model | yes | planned |
| `docs/technical_note/` | The 4–6 page technical note and its figures | yes | planned |
| `data/scenarios/` | Scenario files (`.scn`); small samples only | yes | exists |
| `data/raw_logs/`, `output/` | Raw BlueSky outputs | no (ignored) | planned |
| `data/processed/` | Tidy CSV with metrics | yes | planned |
| `external/bluesky-wiki/` | Local markdown copy of the BlueSky wiki (2022–2023, may be outdated) | **no** (ignored) | exists |
| `configs/`, `src/mixfleet/`, `scripts/`, `tests/` | Study configs, package code, pipeline scripts, tests | yes | planned |

## Outside the repo (siblings, in `TUD\`)

| Path | Purpose |
|------|---------|
| `..\.venv` | Python 3.12 virtual environment (never edit by hand; recreate from `requirements.txt` if needed) |
| `..\bluesky-src` | Clone of the BlueSky repository, reference only; may differ from the installed 1.1.1 |

The code that actually runs is the installed package in `..\.venv\Lib\site-packages\bluesky`.
