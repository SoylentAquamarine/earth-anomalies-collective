# SQ-1 — the sourcing and reproducibility protocol, finally written

**Trigger:** SQ-1 is this project's own explicitly stated blocking task, still undone after two cycles of
SQ-3 (prior-claims catalog) work happening around it. Genuinely overdue to close.

## What's already known / not done yet

Already known: the required fields (coordinates, provider, date, zoom) were already named in
`config/sidequests.md`'s own SQ-1 scope. Not done: freezing the actual format, or verifying which
providers are actually usable without an account — the scope explicitly calls for checking this, not
assuming it.

## Method and why it's non-circular

Rather than assert provider accessibility from memory, directly tested the one most central to this
project's own name (Google Earth) by loading its actual Web URL format and confirming it renders without
a login wall, and searched for the others' access requirements, disclosing search-tier vs. verified-tier
clearly rather than blending them.

## Result

**Directly verified**: Google Earth Web's own URL scheme
(`https://earth.google.com/web/@<lat>,<lon>,<alt>a,<distance>d,<heading>h,<tilt>t,<roll>r`) loads and
renders the standard Earth viewer with no login wall — confirmed by direct navigation in this session's
own browser tool, not assumed. This is the citation format recommended as primary.

**Search-tier only, disclosed as such**: Sentinel Hub's EO Browser appears to support basic browsing
without an account, with a free registration required only for advanced features (time-lapse, data
processing) — sourced from UN-SPIDER's listing and Sentinel Hub's own marketing page, not independently
tested this cycle. USGS Earth Explorer and NASA Worldview's access requirements were **not found** in
search results and are **not verified** — flagged explicitly rather than filled in from assumption.

## Honesty precommitment

The protocol below states exactly what's verified vs. not, and the "not yet verified" providers are
listed as candidates only, not treated as confirmed-usable.

## Decision

Enough is verified to freeze a working protocol with Google Earth as the primary, confirmed-accessible
citation method — the others remain named but explicitly flagged for future verification before being
relied upon as a candidate's sole source.
