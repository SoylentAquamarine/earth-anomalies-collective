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

## Natural-formation patterns

**Three of the original six bootstrap categories are now directly cited; three remain unverified
placeholders** — see `logs/2026-10-10-sq2-natural-formation-patterns-first-citations.md` for full sourcing.

- **Karst topography / sinkholes** (directly fetched, primary tier: USGS Water Science School). Form where
  groundwater dissolves soluble bedrock (limestone, carbonate rock, salt beds), creating underground
  cavities; collapse occurs when the overlying land loses support, sometimes triggered by groundwater
  pumping, construction, or added load. Shapes vary — "shallow bowls or saucers" to vertical-walled pits,
  sometimes eroding into shallower bowl depressions over time. **Directly relevant to circular/depression
  "anomaly" claims on land**, the land-imagery analog of the bathymetric section's own caution above.
- **Patterned ground / "fairy circles"** (directly fetched, secondary-but-specific tier: ScienceAlert's
  reporting on Getzin et al., *Journal of Ecology*, 2020). Leading mechanism: a Turing-type
  self-organization pattern from grasses competing for scarce water in arid environments — bare circles
  channel runoff to surrounding vegetation. Evidenced by drone surveys and soil-moisture sensors near
  Newman, Western Australia; found that healthier, more moisture-dependent grasses correlate more strongly
  with the circles. **Explicitly disclosed as still actively debated**, not settled — rival termite and
  toxic-chemical hypotheses exist, and the Australian find specifically weakened the termite explanation
  (no termite link found there). The paper's own authors state more field work is needed.
- **Salt-pan polygon cracking** (search-synthesis tier, multiple cross-checked sources). Classic
  desiccation-cracking (surface drying → shrinkage → tensile stress → propagating cracks meeting to form
  polygons) explains clay/mud playas well, but is **actively disputed specifically for salt crusts** —
  salt's solubility and widely varying crust thickness undermine a simple desiccation account for the
  typically consistent 1-2 m polygon diameters observed. Competing mechanisms proposed: thermal
  contraction (analogous to basalt columnar jointing), halite crystal growth buckling the crust from below,
  and brine-driven ridge formation along crack boundaries (a 2023 modelling paper). **No single mechanism
  is settled** — recorded honestly as genuinely open science, not resolved by this project. The same
  cracking-pattern family is independently used as evidence for ancient playas on Mars (chloride-bearing
  terrain analysis), a useful cross-reference for recognizing the pattern, not a claim about Earth anomalies.

- **Geological fault lines / lineaments** (search-synthesis tier, cross-checked against NASA/USGS-sourced
  reporting). "Lineament" is the neutral term geologists use for any straight linear feature in imagery,
  tectonic or not; a fault **scarp** (a step in the surface from fault movement) is the strongest visual
  sign, especially combined with offset streams/ridges/valleys. **Explicitly disclosed as misleading on its
  own**: documented real cases exist where a linear scarp was tested and found to be a non-tectonic feature
  instead — an ancient shoreline (south Tehran studies) or a possible wave-cut feature (near Mobile Bay),
  not a fault at all. Confirmation requires fieldwork/trenching/geophysics, not imagery alone. **Directly
  relevant**: a straight-line "anomaly" claim should be checked for offset-drainage evidence, not just
  visual straightness.
- **River oxbow lakes / meander scars** (search-synthesis tier, cross-checked against Britannica).
  Erosion on a meander's outer bank plus deposition on the inner bank narrows the neck between two bends
  until a flood cuts through, isolating the old loop as an oxbow lake; over time it silts in, becoming a
  meander scar — visible on flat farmland as a crescent-shaped depression or a vegetation-color difference,
  not a buried structure. A river's meander-scar density is itself a standard proxy for its geological
  maturity.
- **Agricultural center-pivot and contour patterns** (search-synthesis tier, cross-checked against USGS
  imagery documentation and a NASA-quoted news report on Egyptian Sahara examples). Center-pivot irrigation
  sweeps a fixed radius around a central well, producing the characteristic circular field pattern (visible
  even in deserts, drawing on aquifer groundwater); gravity-fed channel irrigation instead produces
  rectangular patterns. **Not every circular or geometric agricultural field is a pivot** — worth checking
  which irrigation method is locally plausible rather than assuming.

- **Volcanic calderas mistaken for impact craters** (directly fetched, primary tier: NASA Earth
  Observatory). Both produce circular/oblong depressions, but by opposite mechanisms: a caldera forms when
  an emptied underground magma chamber's roof collapses after an eruption (volcanic, "from below"); an
  impact crater forms when a meteor strikes "from above." NASA's own paired example (Emi Koussi, a shield
  volcano with three overlapping eruption-formed calderas, and the Aorounga impact crater, ~110 km away,
  dated to a meteor impact ~345-370 million years ago) is directly citable for distinguishing the two in
  practice. **Documented real-world confusion cases**: a circular feature in Venezuela's Guiana Shield was
  proposed as a possible impact crater from 1980s aerial/radar imagery, but modern elevation data showed it
  lacks diagnostic impact features and is instead the Nuria ring dike, a known intrusive igneous structure
  — the study's own authors note that limited-resolution imagery and simple circular planform can bias
  interpretation toward "impact" without the fieldwork to check it. A systematic Google Earth survey of
  Morocco similarly found many circular structures attributable to magmatic/tectonic processes,
  bioconstruction, or human activity, not impacts — concluding remote-sensing imagery shouldn't be used in
  isolation from other data. **Diagnostic difference worth naming**: impact craters typically show raised
  rims and ejecta; calderas typically lack them.

**All seven original bootstrap natural-formation categories are now cited.** The entire
human-made-explanations section and land-imagery-pipeline-artifacts section (cloud/shadow, stitching
seams, 3D-mesh glitches) remain completely untouched — the clearest next unclaimed thread.

## Human-made explanations (not yet independently verified this cycle)

- Military/industrial test ranges, land-art installations, solar/wind farm arrays, quarry/mining
  operations, abandoned infrastructure. Same status as above — bootstrap-era list, not yet cited.

## Land-imagery pipeline artifacts (not yet covered this cycle)

Cloud/shadow misclassification, flight-pass stitching seams, 3D-mesh rendering glitches specific to
terrain-view rendering. Named in the project's own scope (`config/sidequests.md` SQ-2) but not yet
researched — a clear next-pass target.
