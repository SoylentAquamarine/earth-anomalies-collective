# SQ-2 — the mundane-explanation/imagery-artifact reference catalog, first pass

**Trigger:** flagged last cycle as the natural next unclaimed thread, since SQ-1 and SQ-3 both have real
first-pass work and the Skeptic role (per `agents/skeptic.md`) needs this reference before any candidate
evaluation can responsibly proceed.

## What's already known / not done yet

Already known: the project's own scaffolding named categories to document (elevation-data spikes,
cloud/shadow misclassification, stitching seams, underwater-rendering errors) from general background
knowledge, explicitly flagged as not yet verified. Not done: finding real, citable documentation for any
of them.

## Method and why it's non-circular

Searched for documented bathymetric/imagery artifact cases, then directly fetched the single most
authoritative available source found (GEBCO — the actual international body responsible for global
bathymetric gridding) rather than relying on search-synthesis summaries or hobbyist blog posts.

## Result

**Directly fetched, primary-tier**: GEBCO's own published data-set errata page
(`gebco.net/data_and_products/gridded_bathymetry_data/data_set_errata`) — a maintained, dated, versioned
list of specific documented artifacts in the actual bathymetric data Google Earth and similar platforms
draw from, with real coordinates and named causes. This directly upgrades the scaffolding's
general-knowledge claim about "bathymetric survey-track artifacts" to a primary, citable source with
dozens of specific, dated examples and a stated general cause list (erroneous source soundings, sparse
shallow-water data forcing interpolation, navigation-trackline distortion, mismatched source-dataset
vertical datums, incorrect processing/labeling).

**One particularly notable, independently famous case found in the same source**: "Sandy Island," a
phantom island in the Coral Sea that appeared on charts and in Google Earth's own data for years — GEBCO's
own page states it was "included via coastline and topography datasets, although a later cruise found it
does not exist." This is a well-documented, widely-reported real case of a geographic feature that was
genuinely not there, caused by source-data error rather than any rendering glitch — a useful, concrete,
citable example of exactly the kind of "mundane explanation" category this project's Skeptic role needs
on hand.

**The Geological Society's own "Ask a Geologist" page**, which search results indicated discussed the same
ship-track grid-line phenomenon with a named geologist (Tony Watts), **returned HTTP 404** on direct fetch
— likely reorganized or removed. Not independently confirmed this cycle; the GEBCO source above is
stronger anyway (primary institutional data rather than a secondary explainer).

## Honesty precommitment

This is a first pass covering bathymetric/ocean-floor artifacts specifically — not yet the full scope
named in SQ-2 (cloud/shadow misclassification, flight-pass stitching seams on land, 3D-mesh rendering
glitches specifically). Disclosed as partial, not a complete catalog.

## Decision

Enough real, citable, primary-tier material exists now to write `data/explanation-reference.md`'s
bathymetric-artifact section properly. Land-imagery artifact categories (cloud/shadow, stitching seams,
3D-mesh glitches) remain for a future pass.
