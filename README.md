# Threat2Detection - site data

This repository is the data feed of **https://threat2detection.netlify.app**. It holds no application code.

- The [`site-data`](https://github.com/Halfinity/threat2detection-data/tree/site-data) branch contains the JSON files the site reads: the trending threats, each
  with its YARA-L 2.0 rule and standard SQL query, and the figures on the About page.
- [`.github/workflows/refresh.yml`](.github/workflows/refresh.yml) rebuilds that branch every 30 minutes from the live
  public sources. GitHub runs scheduled jobs on a best-effort basis, so a refresh can occasionally be late; the site
  shows when the data was last updated.

## Data sources and attribution

CISA KEV and NVD data are U.S. Government works. EPSS scores © FIRST, used per FIRST's terms. GitHub Security
Advisories are CC-BY 4.0. MITRE ATT&CK® is a registered trademark of The MITRE Corporation; ATT&CK data © MITRE,
used under the ATT&CK Terms of Use. Research feed items are published as title, link, date and a short summary
only, always linking to the original publication.

Detection rules and queries by [0xHalfin](https://threat2detection.netlify.app/about). Rules marked as drafts are
generated automatically and must be reviewed before use.
