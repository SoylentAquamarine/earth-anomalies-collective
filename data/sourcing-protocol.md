# Sourcing and reproducibility protocol

The frozen citation format every catalogued candidate must use. See
`logs/2026-10-10-sq1-sourcing-protocol.md` for verification method and what's confirmed vs. not.

## Required fields for every candidate

1. **Coordinates** — decimal degrees, minimum 5 decimal places (e.g. `27.51234, -33.49876`), WGS84.
2. **Imagery provider** — named explicitly (see Providers below); never left implicit.
3. **Acquisition/capture date** — the specific date if the provider exposes one, or the best-available
   date range if it doesn't, explicitly labeled as a range rather than presented as precise.
4. **Zoom level / ground resolution** — as exposed by the provider, or an approximate scale bar reading
   if not.
5. **Direct link**, where the provider supports one (see below) — the single most important field, since
   it's what actually makes a claim reproducible by a second party.

## Providers

| Provider | Access | Direct-link support | Historical-date browsing |
|---|---|---|---|
| **Google Earth Web** | **Verified, no account required** (confirmed by direct navigation, 2026-10-10) | Yes — `https://earth.google.com/web/@<lat>,<lon>,<alt>a,<distance>d,<heading>h,<tilt>t,<roll>r` loads the exact view | Supported via the in-app historical-imagery timeline for many locations (not independently re-verified this cycle) |
| **Google Maps** | No account required for basic viewing (general knowledge, not independently re-tested this cycle) | Yes, standard `maps.google.com/?q=<lat>,<lon>` or satellite-view share links | Limited compared to Earth |
| **Sentinel Hub EO Browser** | **Search-tier only**: basic browsing reportedly works without an account; a free registration unlocks advanced features (time-lapse, processing) — not independently tested | Has its own shareable-view links (not verified this cycle) | Yes, this is one of its core features (not independently verified this cycle) |
| **USGS Earth Explorer** | **Not verified this cycle** — commonly described elsewhere as requiring a free account for data download; not confirmed here | Not verified | Not verified |
| **NASA Worldview** | **Not verified this cycle** | Not verified | Yes, this is one of its core features (not independently verified this cycle) |

**Primary recommendation**: cite Google Earth Web's direct-link URL format wherever possible — it's the
only provider in this table actually confirmed, by direct test, to work without an account. Treat the
others as candidates needing their own verification pass before a candidate record relies on them as its
sole source.

## Intake template (for SQ-4's candidate records)

```markdown
## Candidate: <short name>

**Coordinates:** <lat>, <lon>
**Provider:** <name, from the table above>
**Date:** <specific date or range, labeled>
**Zoom/resolution:** <value>
**Direct link:** <url, or "not supported by this provider">
**Origin of claim:** <who/where this was first proposed, with a citation>
**Evidence-ladder status:** Proposed | Sourced | Explanation search run | Cross-checked | Resolved | Currently Unexplained
```

## Standing rule, restated

Never bulk-download imagery tiles or datasets — this protocol works entirely by citing a provider's own
public viewer/link, never by retrieving raw tile data.
