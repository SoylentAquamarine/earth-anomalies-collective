# SQ-2: second land-imagery-pipeline-artifacts citation — 3D-mesh "melting" glitches

## Precommitment self-review (written before research)

**Known:** the land-imagery-pipeline-artifacts section got its first citation last cycle
(multi-provider stitching seams, the Suez Canal case). Its own named sub-category "3D-mesh
glitches" remained uncited. A general search for this phenomenon surfaced a specific, well-
documented, named case: Google Earth's "melting bridges" effect.

**Not done yet:** no source on the 3D-mesh-glitch phenomenon specifically had been fetched.

**Design and why it's non-circular:** search for the documented phenomenon, then directly fetch
a source quoting the artist/researcher who specifically catalogued and named it (Clement Valla's
"Postcards from Google Earth," 2013), rather than relying on a search-engine's own synthesis.

**Honesty precommitment:** disclose which specific fetch attempts succeeded vs. failed, and
report Valla's own framing exactly rather than paraphrasing it into a cleaner-sounding claim.

## Findings

**The phenomenon**: bridges, roads, and other elevated structures in Google Earth's 3D view
appear to "melt" or dip down into the ravines/valleys beneath them — most famously documented
on the Golden Gate Bridge. Clement Valla catalogued and named this effect in his 2013 project
"Postcards from Google Earth."

**Directly fetched** (an old Rhizome editorial piece discussing Valla's own essay, after two
other fetch attempts — Smithsonian Magazine, HTTP 403; Discover Magazine, page had no article
text — were blocked or empty, disclosed rather than silently skipped): Valla's own framing,
quoted directly, is that these are **not glitches**: "They are the absolute logical result of
the system." He calls them an "edge condition" and an "anomaly," not an error — "seams" that
reveal imagery built from "dynamic, ever-changing data from a myriad of different sources"
combined into "a seamless illusion."

**The underlying mechanism** (from the broader search, cross-checked across multiple sources
describing the same effect consistently, though not every individual source was itself directly
fetched): Google's 3D view drapes aerial/satellite photo textures over a terrain model. When
that terrain model doesn't separately model elevated man-made structures (bridges, overpasses)
as solid objects above the ground, the flat photo texture for the bridge surface gets stretched
down to follow the terrain mesh beneath it instead — producing the "melting" appearance. This
is a structural consequence of how texture-mapped 3D terrain rendering works, not a data error
or a location-specific anomaly.

## Outcome

A second, well-documented, named citation for the land-imagery-pipeline-artifacts section's own
"3D-mesh glitches" sub-category, directly quoting the person who specifically catalogued the
phenomenon rather than relying on secondhand paraphrase.

## Limitation disclosed

Two of three fetch attempts for this specific case failed (Smithsonian 403, Discover Magazine
empty) — the successful fetch is a secondary discussion of Valla's essay, not Valla's original
essay itself, though it quotes him directly in several places. The underlying texture-draping
mechanism description is cross-checked across multiple consistent search results but not
independently verified via a single authoritative direct fetch this cycle.
