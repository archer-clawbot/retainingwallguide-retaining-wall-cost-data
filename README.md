# Retaining Wall Cost Register (US, 2026)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23550672.svg)](https://doi.org/10.5281/zenodo.23550672)

Published by **RetainingWallGuide** (https://retainingwallguide.com/). This GitHub repository is a mirror; the canonical, versioned release is on Zenodo.

- **DOI:** [10.5281/zenodo.23550672](https://doi.org/10.5281/zenodo.23550672)
- **Zenodo record:** https://zenodo.org/records/23550672
- **Data page:** https://retainingwallguide.com/retaining-wall-cost/
- **License:** CC BY 4.0 (see LICENSE)

## How to cite
RetainingWallGuide. *Retaining Wall Cost Register (US, 2026)*. Zenodo. https://doi.org/10.5281/zenodo.23550672

---

# Retaining Wall Cost Register (US, 2026)

Compiled by **RetainingWallGuide** (retainingwallguide.com). Version 2026-10-21. **Draft — not yet published.**

A register of individual prices that US contractors and consumer cost guides publish on public web pages for retaining wall installation, repair and replacement. Each row is one published figure with its unit, scope, geography, publisher, source URL, source date, retrieval date and a short verbatim quote of the figure.

- **File:** `retaining-wall-cost-register.csv` (53 rows)
- **Coverage:** 53 rows from 10 source URLs and 7 independent businesses; 20 primary-tier rows and 33 secondary-tier rows; local rows cover CA, GA, MN, SC.
- **Build:** `python3 src/build.py` re-verifies every quote against the raw snapshots and fails if any quote or number is missing.
- **Docs:** METHODS.md, DATA-DICTIONARY.md, FINDINGS.md, raw/SOURCES.md
- **License:** CC BY 4.0 for the compilation (see LICENSE). Underlying figures belong to their publishers and are cited, not relicensed.

Not a quote, survey or representative sample. Do not average rows across different units, scopes or geographies.

Cite as: RetainingWallGuide (2026). *Retaining Wall Cost Register (US, 2026)* (Version 2026-10-21) [Data set].
