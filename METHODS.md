# Methods: Retaining Wall Cost Register (US, 2026)

## Collection
- **Starting list:** the outbound sources cited on retainingwallguide.com's live cost pages (/retaining-wall-cost/, /retaining-wall-repair-cost/, /retaining-wall-replacement-cost/), plus contractor price pages found by web search on 2026-10-21.
- **How:** each page was fetched live on 2026-10-21 (America/Chicago); the raw HTML and a text extraction were kept locally (raw/, not redistributed). Figures were recorded by hand into `src/build.py` with a short verbatim quote. The build normalizes whitespace and dashes and **fails** unless (a) the quote appears in that page's text and (b) every number in the row appears inside the quote.
- No figures came from calls, quote requests, forms, logins or paywalled content.
- **Coverage:** 53 rows from 10 source URLs and 7 independent businesses; 20 primary-tier rows and 33 secondary-tier rows; local rows cover CA, GA, MN, SC.

## Tiers and grouping
- **Primary:** a business publishing its own price, price list, or quoted/completed project.
- **Secondary:** aggregator cost guides (Angi, HomeAdvisor, HomeGuide, etc.), publishers, manufacturers, calculator sites, news reports, and contractor pages that describe general market ranges rather than their own prices.
- Angi and HomeAdvisor share `independent_business` = "Angi Inc." Multiple pages from one company share one value and are not independent corroboration.

## Rules applied
1. No averaging, blending, midpoints or estimates. Any average is the source's own stated figure.
2. Open-ended figures ("$X+", "starting at") are recorded as stated and flagged in `notes`.
3. Scope and unit are recorded with every row; compare rows only when scope, unit and geography match.
4. Undated sources are `Not stated`; dates from page metadata are labeled as such.
5. Only individual figures and short quotes are reproduced; no page text is mirrored.

## Exclusions and gaps
- Not used: city permit pages (Portland, Montgomery County MD) carried no prices; Carrollton TX returned HTTP 403.
- Not used: lakenormanhardscapes.com and cornerstoneexcavationgroup.com restate national guide ranges already in the register (derivative).
- Gap: no primary prices from the Northeast, Midwest (outside MN), Texas, Florida or the Mountain West. No timber or vinyl contractor price lists found.

## Limitations
- Published prices, not transactions; businesses choose what to publish.
- Not representative; few markets and few businesses per market.
- Aggregator ranges are national with undisclosed or partially disclosed methods.
- Point in time; re-check `source_url` before relying on a figure.
