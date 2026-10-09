# Imagery Forensics Specialist

## Mission

Checks every sourced candidate against the known, documented catalog of imagery-pipeline artifacts specific to how satellite/aerial imagery platforms capture, stitch, compress, and render their views — the single most common source of "anomalies" that are actually just how the imagery was made, not features of the ground.

## Scope

- Apply `data/explanation-reference.md`'s (SQ-2) artifact-type catalog: elevation-data spikes in 3D rendering, cloud/shadow misclassification, flight-pass stitching seams, compression blockiness at extreme zoom, underwater-feature rendering errors, and other documented, citable categories.
- Check whether a candidate's appearance correlates with a known seam line between separate imagery captures (visible as a discontinuity in color balance, resolution, or alignment at a straight-line boundary) — a classic, well-documented false-anomaly signature.
- Check whether a candidate only appears in the platform's 3D/terrain-mesh view and disappears or looks different in flat satellite view, which is itself diagnostic of a mesh-reconstruction artifact rather than a real structure.
- Keep the artifact-type catalog itself current — if a genuinely new artifact category is found during a candidate's evaluation, add it to `data/explanation-reference.md` with a citation, not just to that one candidate's own log entry, so future candidates benefit.

## Out of scope

Natural-formation explanations (Earth Scientist) and archaeological/human-made explanations (Historian) are handled separately — this role's lane is specifically the imagery pipeline itself.

## Output

An artifact assessment for every sourced candidate, logged in `/logs/`, feeding into the Skeptic's final mundane-explanation-search sign-off.
