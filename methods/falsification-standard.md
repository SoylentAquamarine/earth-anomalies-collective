# Evaluation and Promotion Standard

This is the minimum bar for moving a candidate anomaly up the evidence ladder in `config/research-department.md`, and for what counts as a reportable "Confirmed Finding" in `knowledge-base/state.md`. This project's domain doesn't have a single decisive "translation" moment the way a decipherment project does — its standard of rigor is instead about **not manufacturing a false positive**, since the single most common and most publicly documented failure mode in this space is exactly that.

## Minimum bar for a Confirmed Finding

A "Confirmed Finding" here is a sourced observation or a resolved explanation — not a claim that something paranormal or undiscovered exists. Before a PR adds an entry to `knowledge-base/state.md`'s Confirmed Findings, it should have:

- exact coordinates (minimum 5 decimal places), imagery provider, acquisition date (or range), and zoom level, per `data/sourcing-protocol.md`;
- for a claimed explanation: a specific, citable source (a geological reference, a documented artifact-type citation, a verifiable human-made-feature record) — not just this project's own assertion that it "looks like" something;
- for a "currently unexplained" classification: explicit, disclosed confirmation that the natural-formation check, the imagery-artifact check, and the prior-claims/human-made check were all actually performed, by name, with their individual results — not merely that no one happened to think of an explanation;
- cross-checking across at least one additional independent imagery source or capture date, with the result disclosed either way.

## Required candidate record

Before a candidate can advance past "Sourced" on the evidence ladder, record:

1. **Claim** — the specific feature claimed, phrased narrowly enough to check (not "something weird here," but what, specifically, is claimed to be unusual).
2. **Origin** — where this claim came from (a specific person, post, video, or this project's own observation) and when it was first circulated, if known.
3. **Alternatives considered** — at minimum, the relevant categories from `data/explanation-reference.md`: natural-formation, imagery-pipeline artifact, and human-made/archaeological.
4. **What would change the classification** — what specific evidence (a different imagery source showing the same thing, a cited geological survey, a located prior debunking) would move this candidate to Resolved, and what would be needed to responsibly call it Currently Unexplained.
5. **Units and scope** — the exact location, the imagery sources actually checked, and what wasn't checked (be explicit about gaps rather than implying completeness).

## Evidence required to reach "Currently Unexplained"

A candidate can be classified "Currently Unexplained" only when all of the following are present and disclosed:

- sourced per SQ-1's protocol, with cross-checking across at least one additional independent provider or capture date;
- the Earth Scientist's natural-formation assessment is on record, with its specific negative result (which patterns were checked and ruled out, not just "none found");
- the Imagery Forensics specialist's artifact assessment is on record, same standard;
- the Historian's prior-claims/human-made assessment is on record, same standard, including a check against `data/prior-claims-catalog.md` for whether this exact claim has already been examined elsewhere;
- the Skeptic has signed off that the search was genuinely exhausted, not merely attempted;
- a statement of what this classification does **not** claim — specifically, that "currently unexplained" is not evidence for any particular alternative explanation (paranormal, extraterrestrial, or otherwise), only an honest statement that a real search didn't find a mundane one yet.

## Automatic stop conditions

Do not advance a candidate, or log it as unexplained, when any of these applies:

- coordinates are approximate, missing, or not independently reproducible;
- only one imagery source or one capture date was checked;
- the natural-formation, artifact, or human-made checks were skipped or only nominally performed;
- the candidate wasn't checked against `data/prior-claims-catalog.md` for a prior resolution;
- the writeup drifts into speculation about origin, purpose, or intent beyond what the imagery itself supports;
- the writeup identifies, or could reasonably be used to identify, a private individual or their activity rather than a place;
- the writeup could function as guidance toward an unauthorized real-world site visit.

## Current consequence

At launch, the repository has no catalogued candidates and no resolved or unexplained entries — this is a genuine bootstrap state. The first substantive work is the sourcing protocol and the prior-claims catalog (`config/sidequests.md`, SQ-1 and SQ-3), which are themselves infrastructure, not findings.
