# Data

Source material and catalogs for the project — coordinates, citations, and this project's own written analysis. No bulk imagery is ever stored here.

## Present

Nothing yet. See `config/sidequests.md` SQ-1 (sourcing protocol) and SQ-3 (prior-claims catalog) — both are foundational groundwork before candidate evaluation can begin.

## Needed

- **`sourcing-protocol.md`** (SQ-1) — the frozen citation format (coordinates, provider, date, zoom) and the intake template every candidate record uses.
- **`explanation-reference.md`** (SQ-2) — the cited catalog of known imagery-pipeline artifacts and natural-formation patterns the Skeptic and other roles check every candidate against.
- **`prior-claims-catalog.md`** (SQ-3) — the catalog of previously publicized "Google Earth anomaly" claims and their documented resolution status.
- **`candidate-intake.md`** (SQ-4, or one file per candidate once the catalog grows) — the live queue of candidates and their evidence-ladder status.

## Tooling

- **`scripts/index_corpus_qdrant.py`** — embeds this repo's own `logs/`,
  `comms/`, `knowledge-base/state.md`, and `methods/` into a Qdrant vector
  collection (`earth-anomalies-collective`) via the linuxbox's
  `nomic-embed-text` model, for semantic search/navigation over this
  project's own prior work. Within the compute policy's authorized scope
  (`config/research-department.md`): a navigation aid only, never a
  substitute for Claude/ChatGPT's own research judgment or adversarial
  review. Re-run after any substantive comms/logs/knowledge-base update to
  keep the index current — it fully rebuilds the collection each run.

## Convention

Any file added here should note its source URL, retrieval date, and (where applicable) a checksum or exact version in a companion note, so provenance is never lost. This project never bulk-downloads imagery tiles or datasets — only coordinates, citations, and links to a provider's own public viewer are stored here.
