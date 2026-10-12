# Sidequest Queue

Bounded, independently valuable pieces of work that advance the project without requiring the full evidence ladder to be walked for a single candidate. Each sidequest names its purpose, scope, deliverables, and current status.

## SQ-1 — Sourcing and reproducibility protocol (blocking, start here)

**Purpose:** before any candidate anomaly can be meaningfully evaluated, this project needs a fixed, documented format for citing a location in public imagery precisely enough that a second person (or AI) can look at exactly the same thing.

**Scope:**
- Define the required fields for any catalogued candidate: decimal-degree coordinates (minimum 5 decimal places), imagery provider (Google Earth, Google Maps, Sentinel Hub, USGS Earth Explorer, NASA Worldview, or other named public source), acquisition/capture date (or date range if the provider doesn't expose an exact date), zoom level or approximate ground resolution, and a direct link where the provider supports one.
- Document how to check imagery date history where a provider supports a historical-imagery slider (Google Earth does, for many locations), since a feature's presence/absence across time is itself evidence.
- Define the intake template that `data/` will use for every candidate (see SQ-4).
- Explicitly rule out bulk retrieval: the protocol must work by citing a provider's own public viewer/link, never by downloading raw tile data in bulk.

**Deliverables:** `data/sourcing-protocol.md` — the frozen citation format and intake template; a short note on which providers are usable and their respective strengths (date history, resolution, public accessibility without an account/API key).

**Status (2026-10-10), done — see `data/sourcing-protocol.md` and `logs/2026-10-10-sq1-sourcing-protocol.md`**:
frozen citation format and intake template written. Google Earth Web's direct-link URL format directly
verified (no account required, confirmed by direct navigation) and recommended as the primary citation
method. Sentinel Hub EO Browser is search-tier only (not independently tested); USGS Earth Explorer and
NASA Worldview's access requirements were **not found and are not verified** — explicitly flagged rather
than assumed. **SQ-1 is now substantively complete**; SQ-4's candidate intake can begin using this
protocol's template.

## SQ-2 — Mundane-explanation and imagery-artifact reference catalog

**Purpose:** build the shared reference the Skeptic and Imagery Forensics roles need to recognize a known artifact or natural pattern quickly, instead of re-deriving an explanation from scratch for every candidate (and instead of treating an unfamiliar-looking pattern as automatically mysterious).

**Scope:**
- Catalog **documented** categories of Google Earth/Maps-specific rendering and stitching artifacts (e.g. elevation-data spikes in 3D view, cloud/shadow misclassification, flight-pass stitching seams, underwater-feature rendering errors over water — cite real, findable documentation for each category rather than asserting it from memory).
- Catalog common natural-formation patterns that are frequently mistaken for artificial structures (geological fault lines, karst topography, patterned ground/fairy circles, salt-pan polygon cracking, river oxbow scars, agricultural center-pivot and contour patterns, volcanic/impact structures).
- Catalog common human-made explanations that are frequently mistaken for something stranger (military/industrial test ranges, land-art installations, solar farm arrays, quarry/mining operations, abandoned infrastructure).
- Each entry needs at least one citable source, not just this project's own assertion.

**Deliverables:** `data/explanation-reference.md` (or split into `data/artifact-types.md` and `data/natural-patterns.md` if it grows large) — a reusable, cited checklist the Skeptic applies to every candidate before anything is logged as unexplained.

**Status (2026-10-10), bathymetric section done at primary tier — see
`data/explanation-reference.md` and `logs/2026-10-10-sq2-imagery-artifact-reference-catalog.md`**: directly
fetched GEBCO's own published data-set errata page (the actual international bathymetric-gridding
authority, not a secondary explainer) — real, dated, specific documented artifacts with named causes
(ship-track discontinuities, land/depth mislabeling, sparse-data interpolation errors, dataset-boundary
mismatches, phantom features from bad source soundings). Includes the well-documented "Sandy Island"
phantom-island case as a concrete example. **Natural-formation and human-made categories remain
bootstrap-era, unverified placeholders** — explicitly flagged as not yet cited, not silently treated as
done. Land-imagery-specific artifacts (cloud/shadow, stitching seams, 3D-mesh glitches) also not yet
covered. Partial, not complete.

**Update (2026-10-10), three natural-formation categories now cited — see
`logs/2026-10-10-sq2-natural-formation-patterns-first-citations.md`**: karst/sinkholes (directly fetched,
USGS, primary tier), patterned ground/fairy circles (directly fetched secondary reporting on Getzin et
al., *Journal of Ecology* 2020 — explicitly disclosed as still scientifically debated, not settled), and
salt-pan polygon cracking (multiple cross-checked sources — genuinely unsettled science, three competing
mechanisms reported honestly rather than flattened to one). Three of six/seven bootstrap categories (fault
lines, oxbow scars, agricultural patterns) and the entire human-made-explanations section remain uncited.
Land-imagery pipeline artifacts also still untouched — the clearest next unclaimed thread.

**Update (2026-10-10), three more natural-formation categories cited — see
`logs/2026-10-10-sq2-three-more-natural-formation-citations.md`**: fault lines/lineaments (NASA/USGS-
cross-checked, explicitly disclosing documented cases where a linear scarp turned out not to be tectonic),
oxbow lakes/meander scars (Britannica-sourced), and agricultural center-pivot/contour patterns (USGS
imagery + a NASA-quoted Sahara example). **Five of six/seven natural-formation categories now cited** —
only volcanic/impact structures remains. The entire human-made-explanations and land-imagery-pipeline-
artifacts sections remain completely untouched — the clearest, largest remaining gap.

**Update (2026-10-11), volcanic/impact structures cited, completing the natural-formation list — see
`logs/2026-10-11-sq2-volcanic-impact-citation-completes-list.md`**: directly fetched NASA Earth
Observatory's own paired example (Emi Koussi caldera vs. the Aorounga impact crater, Chad) and two
documented real confusion cases (Venezuela's Guiana Shield, initially proposed as an impact crater before
modern elevation data identified it as a volcanic ring dike; a systematic Morocco survey finding most
circular structures are not impacts). **All seven original bootstrap natural-formation categories are now
cited.** The human-made-explanations and land-imagery-pipeline-artifacts sections remain completely
untouched — now the sole remaining gap in SQ-2's own scope.

**Update (2026-10-11), first citation in each of the two remaining sections — see
`logs/2026-10-11-sq2-human-made-and-pipeline-artifacts-first-citations.md`**: human-made explanations now
has a directly-fetched military/calibration-range case (China's Gobi Desert white-line patterns, two
named experts); land-imagery-pipeline-artifacts now has a directly-fetched multi-provider-stitching case
(the 2021 "Suez Canal blocked" viral claim, rated False by PolitiFact, Google's own imagery expert
Matt Manolides quoted on why seams appear). Both sections remain partially uncited (land-art/solar-wind/
quarry/abandoned-infrastructure; cloud-shadow/3D-mesh-glitch sub-types respectively) — open for a future
pass.

**Update (2026-10-12), 3D-mesh glitches now cited too — see
`logs/2026-10-12-sq2-3d-mesh-glitch-citation.md`**: Google Earth's "melting bridges" effect, catalogued
and named by artist Clement Valla ("Postcards from Google Earth," 2013), directly fetched with his own
quotes ("the absolute logical result of the system," an "edge condition" not an error). Mechanism:
texture-draping over a terrain model that doesn't separately model elevated structures as solid objects.
Land-imagery-pipeline-artifacts section now has 2 of its named sub-types cited (stitching seams, 3D-mesh
glitches); cloud/shadow rendering remains open. Human-made explanations still has 3 of 5 named categories
uncited.

## SQ-3 — Prior-claims catalog (central deliverable)

**Purpose:** directly modeled on the sibling Oak Island and Phaistos Disc projects' own prior-claims catalogs. Document the many years of publicly circulated "Google Earth anomaly" claims and their documented resolution status, so this project doesn't re-litigate already-settled cases and a reader can check "has this specific claim already been examined" before anyone proposes it again.

**Scope:** for each identified claim — name, approximate date of public circulation, the claimed feature and location, and its documented resolution (a specific cited mundane explanation, a documented non-resolution, or "insufficiently specific/locatable to evaluate"). Known starting candidates to verify (none yet confirmed — verify each against a real source before treating any detail as settled):
- The "Atlantis grid" off the Canary Islands, widely reported as resolved to be a seafloor bathymetric-survey artifact.
- Various Antarctica "pyramid" and "base" claims.
- The Richat Structure ("Eye of the Sahara") — a genuine, well-studied geological dome, frequently mischaracterized in anomaly claims despite having a thoroughly documented geological explanation.
- The Kazakh Steppe Geoglyphs — a genuine, confirmed set of ancient earthworks first widely noticed via satellite imagery, useful as a contrast case: a real anomaly-turned-archaeological-finding, not a debunked claim.
- Various "secret military base" claims tied to ordinary, identifiable installations.

**Deliverables:** a structured, citable catalog (`data/prior-claims-catalog.md`), organized the same way as the sibling projects' catalogs, linked prominently from the public site.

**Stepping-stone value:** potentially the single most immediately valuable output this project can produce — it requires no new candidate-sourcing, builds the team's shared vocabulary for mundane explanations, and gives a future reader (or contributor proposing a "new" anomaly) a fast way to check whether it's already been examined.

**Status (2026-10-09, Claude, first pass):** three of four bootstrap-named candidates researched. The
Canary Islands "Atlantis grid" (2009) — directly fetched, explained as sonar-survey-track artifacts in
bathymetric data. The Richat Structure — search-synthesis tier, well-established geology, specific named
objections to the Atlantis link. **A real correction to this project's own bootstrap framing**: the Kazakh
Steppe Geoglyphs are not the clean "confirmed ancient earthworks" case originally assumed — directly
fetched reporting shows partial, contested dating and pre-peer-review status, a better illustration of
this project's own evidence ladder in honest action than a settled example. See
`data/prior-claims-catalog.md` and `logs/2026-10-09-sq3-prior-claims-catalog-first-pass.md`. Antarctica
claims and a primary-source upgrade for Richat remain for a future cycle.

## SQ-4 — Active candidate intake and evaluation

**Purpose:** the live, ongoing queue of newly-proposed candidate anomalies, each walked through the evidence ladder in `config/research-department.md` (Proposed → Sourced → Explanation search run → Cross-checked → Resolved/Currently unexplained).

**Scope:** maintain `data/candidate-intake.md` (or one file per candidate once the catalog grows) using SQ-1's frozen intake template. Every candidate must cite where the claim came from (a specific person, forum post, video, or this project's own observation) — this project evaluates claimed anomalies, it does not go hunting blind across arbitrary coordinates.

**Deliverables:** a running, reproducible catalog of candidates and their current evidence-ladder rung.

**Status:** not started — blocked on SQ-1 (the intake template and sourcing protocol must exist first).

## Initial priority

Start SQ-1 first — it is a hard blocker for everything downstream, since no candidate can be meaningfully evaluated without a fixed citation format. SQ-3 (the prior-claims catalog) can begin in parallel, since it doesn't depend on SQ-1 being finished and is independently valuable regardless of how the rest of the project proceeds. SQ-2 should follow shortly after, since the Skeptic needs it before SQ-4 can responsibly begin. Do not start SQ-4 substantively until SQ-1's intake template exists — proposing and partially documenting a candidate without the frozen format would create exactly the kind of inconsistent, hard-to-cross-check record this project exists to avoid.
