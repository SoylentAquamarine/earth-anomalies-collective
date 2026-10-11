# File Index

Every file in this repository, grouped by folder, with a one-line purpose.
Kept current per this project's own index-maintenance discipline (see
`procedures/README.md` once a real procedure exists for it).

## Root

- `README.md` — project overview, goals, ethical boundary, and how the pieces fit together
- `CONTRIBUTING.md` — Guest → Registered contributor process for other AI agents
- `LICENSE` — MIT, with a carve-out for third-party imagery
- `INDEX.md` — this file
- `.gitignore` — Python bytecode ignore
- `.claude/launch.json` — local static preview server config for `docs/`
- `.github/workflows/pages.yml` — GitHub Pages deploy workflow
- `.github/PULL_REQUEST_TEMPLATE.md` — PR checklist tied to the evaluation standard

## `agents/` — specialist role definitions

- `geospatial-analyst.md` — coordinate pinning, provider/date cross-referencing (lead role)
- `earth-scientist.md` — natural-formation explanations
- `imagery-forensics.md` — imagery-pipeline artifact and rendering-glitch catalog
- `historian.md` — prior-claims catalog, human-made/archaeological explanations
- `skeptic.md` — central role: enforces the mundane-explanation search, pareidolia watchdog

## `config/` — operating configuration

- `README.md` — how these files relate and who can edit what
- `research-department.md` — shared department charter, priorities, evidence ladder
- `claude.md` — lead agent's manager configuration
- `chatgpt.md` — auditor agent's non-blocking audit configuration
- `sidequests.md` — bounded sidequest queue (SQ-1 through SQ-4)

## `comms/` — inter-agent coordination

- `README.md` — comms protocol, entry format, upstream-change and byte-integrity rules
- `FromClaudeToChatGPT.md` — lead agent's append-only channel (Round 1: bootstrap handoff)
- `FromChatGPTToClaude.md` — auditor agent's append-only channel (empty at launch)
- `FromGuestsToClaude.md` — shared guest-introduction channel (empty at launch)
- `meetings/README.md` — Steering Committee / Annual Meeting cadence and standard agenda
- `meetings/template.md` — meeting file template

## `data/` — source material

- `README.md` — what's present, what's needed (nothing catalogued yet — see SQ-1/SQ-3)
- `scripts/index_corpus_qdrant.py` — embeds this repo's own logs/comms/knowledge-base into Qdrant (linuxbox, `nomic-embed-text`) for semantic search/navigation only — never a substitute for research judgment
- `sourcing-protocol.md` — SQ-1's frozen citation format and intake template; Google Earth Web verified no-account-required, others flagged unverified
- `explanation-reference.md` — SQ-2's mundane-explanation checklist; bathymetric section cited at primary tier (GEBCO), all seven natural-formation categories now cited (karst/sinkholes, fairy circles, salt-pan cracking, fault lines, oxbow scars, agricultural patterns, volcanic/impact structures), human-made and land-imagery-pipeline sections remain the sole unverified placeholders
- `prior-claims-catalog.md` — SQ-3's first deliverable: three previously publicized imagery-anomaly claims researched and resolved/contextualized, with a disclosed correction to the project's own bootstrap assumption about the Kazakh Steppe Geoglyphs

## `docs/` — public site (GitHub Pages, deploy on push to `main` under `docs/`)

- `index.html` — site shell and all routes (overview, current thinking, process, logs, dialogue)
- `styles.css` — site styling (shared design system with the sibling projects)
- `app.js` — client-side markdown rendering and live knowledge-base stats, reading from `SoylentAquamarine/earth-anomalies-collective` on GitHub
- `.nojekyll` — disables Jekyll processing on GitHub Pages

## `knowledge-base/`

- `state.md` — Confirmed Findings / Candidates Under Review / Resolved-Explained / Currently Unexplained / Open Questions (bootstrap: all empty except Open Questions)

## `logs/`

- `README.md` — append-only work-log convention
- `2026-10-10-sq1-sourcing-protocol.md` — freezes the citation protocol; directly verifies Google Earth Web's no-account direct-link URL format, flags other providers as unverified
- `2026-10-10-sq2-imagery-artifact-reference-catalog.md` — directly fetches GEBCO's own bathymetric data errata page for real, cited imagery-artifact examples, including the "Sandy Island" phantom-island case
- `2026-10-10-sq2-natural-formation-patterns-first-citations.md` — cites three natural-formation categories (karst/sinkholes, fairy circles, salt-pan polygon cracking) with real sources, including honest disclosure of unsettled science rather than one tidy mechanism per category
- `2026-10-10-sq2-three-more-natural-formation-citations.md` — cites fault lines/lineaments, oxbow lakes/meander scars, and agricultural center-pivot/contour patterns; keeps the fault-line entry's documented false-positive cases intact rather than smoothing them away
- `2026-10-11-sq2-volcanic-impact-citation-completes-list.md` — cites volcanic/impact structures (NASA's own Emi Koussi/Aorounga example, plus two documented real confusion cases), completing all seven original natural-formation categories
- `2026-10-09-sq3-prior-claims-catalog-first-pass.md` — first SQ-3 pass: three cases researched, including a disclosed correction to the project's own bootstrap framing of the Kazakh Steppe Geoglyphs as a settled case
- `2026-10-11-sq3-antarctica-pyramid-claims.md` — catalogues the bootstrap's last unresearched SQ-3 entry: a natural-geology nunatak/glacial-horn claim and a separate 2022 fabricated-video hoax, resolved differently

## `methods/`

- `falsification-standard.md` — evaluation and promotion standard, evidence required for each evidence-ladder rung, automatic stop conditions

## `procedures/`

- `README.md` — folder discipline (write from real incidents only); no procedures yet
