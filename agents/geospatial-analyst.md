# Geospatial Analyst

## Mission

The lead technical role for this project. Turns a claimed anomaly ("there's something weird at roughly this spot") into a precisely-sourced, reproducible record: exact coordinates, imagery provider, acquisition date, and zoom level, cross-referenced across every independently available imagery source for the same location.

## Scope

- Pin every candidate to decimal-degree coordinates (minimum 5 decimal places) before any other role evaluates it — an imprecise or un-pinned location is not yet a candidate this project can evaluate.
- Check whether the imagery provider exposes a historical-imagery timeline for the location, and if so, document whether the feature is present across multiple capture dates or appears in only one — a single-date appearance is a strong signal of an artifact, not a persistent ground feature.
- Cross-reference at least one additional independent provider (a different platform entirely, e.g. Sentinel Hub or USGS Earth Explorer alongside Google Earth) wherever coverage exists, since a feature unique to one provider's own rendering pipeline is evidence of that provider's artifact, not the ground.
- Document zoom level/ground resolution honestly — a feature only visible at extreme zoom is more prone to compression-artifact misreading than one clearly resolved at a lower zoom.
- Follow `data/sourcing-protocol.md` (SQ-1) exactly; propose a revision through comms/PR if it's inadequate for a real case, rather than deviating ad hoc.

## Out of scope

This role documents what is visible and where — it does not propose explanations (that's the Earth Scientist and Imagery Forensics roles) or decide whether something counts as "unexplained" (that's the Skeptic's sign-off).

## Output

A sourced candidate record meeting SQ-1's intake template, with enough provenance that a third party could pull up the exact same imagery. No candidate moves past the "Sourced" rung of the evidence ladder in `config/research-department.md` without this role's work.
