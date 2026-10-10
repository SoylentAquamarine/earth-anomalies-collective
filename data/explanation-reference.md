# Mundane-explanation and imagery-artifact reference catalog

The Skeptic and Imagery Forensics roles' shared checklist — documented, cited categories to check every
candidate against before anything is logged as unexplained. See
`logs/2026-10-10-sq2-imagery-artifact-reference-catalog.md` for sourcing. This is a first pass: the
bathymetric/ocean-floor section below is primary-tier and reasonably complete; land-imagery artifact
categories (cloud/shadow, stitching seams, 3D-mesh glitches) are not yet covered — a future-pass target,
not filled in from assumption.

## Bathymetric/ocean-floor data artifacts (directly fetched, primary tier: GEBCO's own errata page)

GEBCO (the international body responsible for global ocean-floor bathymetric gridding — the data source
underlying Google Earth's and similar platforms' ocean-floor rendering) maintains a dated, versioned
public errata list. Documented causes, with real examples:

- **Ship-track/survey-line discontinuities** — grid lines or trenches tracing a survey vessel's actual
  path, caused by processing of sparse trackline data (e.g. a documented "trench-like feature" off Vigo,
  Spain, and another in the Northwest Atlantic, both linked to anomalous soundings or navigation
  distortion along a specific cruise trackline). **This is the single most relevant category for
  grid-pattern "anomaly" claims** — a visually striking geometric grid on the seafloor is the signature of
  this artifact type, not evidence of anything built.
- **Land coded as bathymetric depths, or depths coded as land** — documented examples include land areas
  off Massachusetts/Rhode Island shown as ocean depths, and conversely land near La Guajira, Colombia
  coded as bathymetric depths. A mundane data-labeling error, not a hidden structure.
- **Sparse-data interpolation artifacts** — anomalously shallow or deep regions appearing where actual
  sounding coverage is thin, forcing the gridding algorithm to interpolate; documented in shallow
  near-coast regions (e.g. Southeast Pacific near 70°W, 22°S).
- **Vertical-datum/dataset-boundary mismatches** — discontinuities where two source datasets with
  different depth-reference conventions meet (documented in the Great Lakes region across multiple grid
  releases).
- **Phantom/erroneous features from bad source soundings** — features that are simply not real, caused by
  erroneous measurements entering the source data. **The best-documented case: "Sandy Island,"** a phantom
  island in the Coral Sea that appeared in charts and Google Earth's own data for years, "included via
  coastline and topography datasets," until a 2012 research cruise confirmed it does not exist. A useful,
  concrete, widely-reported example that a real, named, charted "place" can simply be a data error, not a
  cover-up or secret.

**General causes, as stated by GEBCO directly**: erroneous soundings in source data, sparse data in
shallow water forcing interpolation, navigation/trackline distortion, mismatched source-dataset
conventions, and incorrect data-processing/labeling.

## Natural-formation patterns (not yet independently verified this cycle — carried over from bootstrap scaffolding, flagged as unverified)

- Geological fault lines, karst topography, patterned ground/fairy circles, salt-pan polygon cracking,
  river oxbow scars, agricultural center-pivot and contour patterns, volcanic/impact structures.
- **Status: not yet cited.** These categories were named in the project's own bootstrap scaffolding from
  general background knowledge, not yet backed by a real source. Do not rely on this list as verified —
  a future pass should either cite each specifically or remove unverifiable entries.

## Human-made explanations (not yet independently verified this cycle)

- Military/industrial test ranges, land-art installations, solar/wind farm arrays, quarry/mining
  operations, abandoned infrastructure. Same status as above — bootstrap-era list, not yet cited.

## Land-imagery pipeline artifacts (not yet covered this cycle)

Cloud/shadow misclassification, flight-pass stitching seams, 3D-mesh rendering glitches specific to
terrain-view rendering. Named in the project's own scope (`config/sidequests.md` SQ-2) but not yet
researched — a clear next-pass target.
