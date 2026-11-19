# SQ-2: Desert Breath citation upgrade — precommitment self-review (written before any fetch)

## Known
Desert Breath (Egypt, 1997, D.A.ST.) is a land-art candidate for the "human-made explanations" category; so far
search-synthesis tier only (nbcnews.com not fetchable). Category stands at 3 of 5 cited.

## Not done yet
No article body has been read; nothing added to data/explanation-reference.md.

## Design and why it's non-circular
Try WebFetch on space.com and csmonitor.com (and the D.A.ST./artist pages if surfaced by a search) with a
prompt that asks only what the page states about who made it, when, size, and how it was publicly identified. The
case was found by search before this step, and I accept or reject it on what the fetched text actually says.
Public artwork only; no private individuals; no site-visit guidance.

## Prediction
Roughly 50% that at least one host resolves with a usable body.

## Honesty precommitment
If a fetch returns the article, cite it with its fetched tier; if every host is blocked, log a disclosed null and
leave land-art uncited. A contradiction of the snippet-derived details will be reported and corrected, not hidden.

## Result (appended after execution) — disclosed null on fetch; search-synthesis corroboration only
One WebSearch plus two WebFetch attempts (livescience.com, en.wikipedia.org): both hosts failed DNS resolution
(not on the session's network allow-list). No article body was read. The search results did add independent
corroboration at snippet level: many unrelated outlets (Live Science, Gizmodo, Colossal, Egyptian Streets,
Euro Weekly News, My Modern Met) list the same creators (D.A.ST. Arteam: Danae Stratou, Alexandra Stratou, Stella
Constantinides), 1997 completion, a double spiral near the Red Sea, and Google Earth users noticing it in Nov 2013.
That strengthens confidence but is still search-synthesis tier, not fetched. Minor discrepancy: location is given as
near Hurghada (Wikipedia snippet) or near El Gouna (others). Not added to data/explanation-reference.md; land-art
stays "candidate found, uncited". Prediction (~50% a host resolves): not met.
Next step: allow-list en.wikipedia.org / livescience.com / space.com for WebFetch, then cite Desert Breath at fetched tier.
