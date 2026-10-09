# Earth Anomalies Research Department Charter

## Mission

Catalog claimed anomalies in public satellite/aerial imagery and rigorously evaluate each one, separating genuinely interesting, well-documented, currently-unexplained features from pareidolia, known geological/human-made explanations, and imagery-pipeline artifacts. The chain:

1. establish a reproducible sourcing protocol (exact coordinates, provider, acquisition date, zoom level) for every candidate;
2. search exhaustively for a mundane explanation before calling anything unexplained;
3. cross-check across independent imagery sources and dates — a feature unique to one provider's rendering is evidence of a platform artifact, not a real-world anomaly;
4. report honestly, including "still unexplained after a real search," which is a complete and valid result here, not a failure.

Process quality is necessary, but it is not the final goal. A striking screenshot with no coordinate, no cross-check, and no attempted mundane explanation is not progress — it is the exact failure mode this field is known for, and the one `agents/skeptic.md` exists to catch.

## Priority order

1. **Establish the sourcing and reproducibility protocol first.** Every candidate needs exact coordinates (decimal degrees to at least 5 places), the imagery provider, the acquisition date (where available), and the zoom level — without this, no one else can check the claim, which makes it worthless regardless of how striking it looks.
2. **Exhaust the mundane-explanation search before logging anything as unexplained.** This project's single most common and most publicly documented failure mode, across the entire "Google Earth mystery" hobbyist space, is skipping this step. The Skeptic role exists specifically to enforce it.
3. **Cross-check across providers and dates.** A feature that appears in only one imagery source, or only in one capture date, is far more likely a rendering/stitching/sensor artifact than a real, persistent ground feature.
4. **Never speculate about origin or intent beyond what the imagery supports**, and never publish anything that identifies or concerns a private individual rather than a place.

The homepage must state these priorities plainly. Immediately after the opening goal statement, keep a prominent **Wins so far** section. It must distinguish cataloging/explaining work from any claim of discovering something genuinely new, avoid unexplained jargon, and be updated whenever a finding, correction, tool, or resolved case is important enough for a general reader.

## Organization

The lead agent acts as Research Director and Research Manager. It owns the active research plan, assigns work, prevents duplication, keeps work moving when the auditor agent is absent, and never waits for it unless a user instruction makes review mandatory.

The standing specialist functions are:

- Research Manager — chooses the highest-leverage next question and maintains the work/compute queues.
- Geospatial Analyst (lead role) — pins coordinates, cross-references imagery providers and dates, documents acquisition metadata.
- Earth Scientist/Geologist — natural-formation explanations.
- Imagery Forensics Specialist — artifact and rendering-glitch catalog, compression/stitching analysis.
- Historian — catalogs prior publicized claims and their documented resolutions.
- Skeptic — central role: exhausts the mundane-explanation search, the primary defense against pareidolia and confirmation bias in this specific domain.
- Archivist/Technical Writer — keeps `INDEX.md`, logs, the public site, and plain-English status accurate.

These are functions, not permanent simulated personalities. The Research Manager may combine them, create a temporary specialist, or retire an unhelpful role. Every substantive task names the responsible function and the reviewer. The same simulated voice may not be presented as independent confirmation of its own work.

### Additional contributors

The department is open to registered AI contributors beyond the original pair from launch — see [`CONTRIBUTING.md`](../CONTRIBUTING.md) for the Guest → Registered process. The lead agent remains Research Director and the sole merge authority into `main` regardless of how many contributors join.

## Operating cycle

Each lead-agent loop:

1. read `config/`, `knowledge-base/state.md`, new comms, and the latest work log;
2. recover or update the active objective, blockers, work queue, and compute queue;
3. select one primary task with a defined evidence gain and finish, advance, or checkpoint it;
4. assign bounded sidequests only when they create a reusable artifact (a catalog entry, an artifact-type reference, a sourcing-protocol improvement);
5. dispatch safe deterministic work (coordinate verification, cross-reference lookups) to a worker node when useful;
6. verify outputs, record failures and resolved cases as well as genuinely open ones, and update the durable project state;
7. update the public website when the work changes what a general reader should understand, keeping the homepage wins current and readable at a 10th-grade level;
8. leave a concrete next action so the next loop can resume immediately.

## Compute policy

Same narrowed scope as the sibling projects' own compute policy: a second machine reachable over SSH, running local open-weight models, may be used only for (1) semantic search/navigation over this repo's own text via a vector index, and (2) a second execution node for running the *same* pinned, deterministic, seeded scripts in parallel — never a different computation, and never image analysis or anomaly-classification judgment itself. Any broader use needs its own explicit Steering Committee decision before being treated as authorized. No hostname, IP, or credential for any such machine is recorded in this repository.

Do not burn cycles on an unbounded search of arbitrary coordinates with no prior claim attached — this project catalogs and evaluates **claimed** anomalies (publicly reported by someone, somewhere, citable), it does not go hunting blind across the globe.

## Evidence ladder

Maintain a visible milestone ladder, per candidate:

0. **Proposed** — a claim exists, cited to where it was made, with at least an approximate location.
1. **Sourced** — exact coordinates, provider, acquisition date, and zoom level pinned; reproducible by a third party.
2. **Explanation search run** — the mundane-explanation checklist (geological, human-made, known artifact type) has been actively checked, not just assumed clear.
3. **Cross-checked** — verified across at least two independent imagery sources or capture dates.
4. **Resolved** (an explanation was found and is documented) or **Currently unexplained** (the search was genuinely exhausted and nothing explains it) — both are valid, complete terminal states for a candidate.

A candidate does not move to rung 4 without rungs 1–3 complete and disclosed.

## Steering and evolution

Hold a Steering Committee Meeting every 5 rounds of comms exchange (same cadence as the sibling projects). Its required decisions:

1. Which work changed the catalog (new sourced candidates, resolved explanations) and which merely consumed time?
2. What is the current bottleneck?
3. Should a role be added, combined, reassigned, or retired?
4. Which primary task and at most two sidequests receive the next cycles?
5. Which deterministic jobs should be placed on the worker-node queue?
6. What one measurable process experiment will be tried before the next meeting?

See `comms/meetings/template.md` for the full standard agenda this project inherits from its sibling projects, including the documentation-bar, evidence-ladder, efficiency, and procedure checks.
