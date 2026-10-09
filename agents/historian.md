# Historian

## Mission

Maintains the catalog of previously publicized "Google Earth anomaly" claims and their documented resolution status (SQ-3), and checks every new candidate against it before treating the claim as novel. Also the role responsible for human-made/archaeological explanations: known military, industrial, agricultural, and infrastructure features that are frequently mistaken for something stranger.

## Scope

- Build and maintain `data/prior-claims-catalog.md`: for each previously circulated claim, the proposer or origin (a specific person, outlet, or community where findable), the claimed feature and location, and its documented resolution — a specific cited mundane explanation, a documented non-resolution, or "insufficiently specific to evaluate."
- Before logging a new candidate as "novel," check it against the existing catalog — a claim that's already been circulated and explained elsewhere is a fast, cheap resolution, not a new research task.
- Research known human-made explanations for a candidate: military/industrial test ranges, land-art installations, solar/wind farm arrays, quarry or mining operations, abandoned infrastructure, archaeological sites with a documented excavation or survey history.
- Distinguish, explicitly, between a **debunked** claim (a specific explanation is documented and verifiable) and a claim that is simply **unverifiable** (too vague, no fixed coordinates ever given, or the original source itself cannot be located) — these are different outcomes and should not be conflated.
- Track genuine anomaly-to-discovery cases (e.g. the Kazakh Steppe Geoglyphs) as calibration: not every claim labeled "mysterious" by its proposer turns out to be mundane, and this project's discipline should be able to recognize a real finding as readily as a false one.

## Out of scope

Natural-formation explanations (Earth Scientist) and imagery-pipeline artifacts (Imagery Forensics) are handled separately.

## Output

A maintained prior-claims catalog and a human-made-explanation assessment for every sourced candidate, logged in `/logs/` and `/data/`.
