# 3GPP Spec Explorer

> An unofficial, community-built navigation aid for the 3GPP technical specification ecosystem.

## Why this exists

The 3GPP specification corpus is one of the most consequential bodies of technical writing in modern engineering — it defines how every cellular network on the planet operates. But the official portal at [3gpp.org](https://www.3gpp.org) is organized around an internal numbering convention (series 21, 23, 25, 36, 38, …) that assumes you already know where to look.

For the people who use these specs every day — RAN engineers, core-network architects, protocol implementers, security researchers, students, standards delegates — finding the right document still means:

- remembering that **5G NR Radio** lives in the **38 series**,
- that **LTE architecture** is in **23**, but **LTE radio** is in **36**,
- that **24 series** holds **NAS signalling** while **29** covers **core-network signalling**,
- and that the boundary between **4G** and **5G** content inside any given series is rarely obvious from the outside.

Newcomers spend weeks building this mental map. Veterans still trip on it.

**This page is an attempt to flatten that learning curve.** It maps the human-friendly terms people actually use — *2G, 3G, 4G, 5G, 6G, Release 18, NAS, security, codecs* — onto the series numbers that 3GPP organizes its work around, and links each one back to the official status report on 3gpp.org.

## What it is

- A **single HTML page** — no backend, no database, no tracking.
- A **curated map**, not a search engine. Every entry is hand-placed.
- A **directory of deep links** to the official 3gpp.org documents. Nothing is mirrored or re-hosted.

## What it is *not*

- **Not affiliated with, endorsed by, or sponsored by 3GPP.**
- **Not a source of specifications.** Every link points back to 3gpp.org. All standards content remains the intellectual property of 3GPP and its Organizational Partners.
- **Not authoritative.** When this page and the official portal disagree, the official portal wins.

## How it should grow over time

The value of a curated map compounds with curation. A few directions worth pursuing:

1. **Deeper series mapping** — drill from a series (e.g. *38*) down to individual specs (*38.211, 38.213, 38.331…*) with a one-line description of each.
2. **Release-aware filtering** — show which specs were introduced or significantly amended in Rel-15 → Rel-19, and what's tentatively scoped for Rel-20.
3. **Cross-references** — for any spec, surface the related specs (e.g. *36.331 ↔ 38.331* for RRC continuity across LTE and NR).
4. **Working-group context** — annotate each series with the responsible TSG/WG (RAN1, RAN2, SA2, CT1…) so newcomers learn the org chart alongside the documents.
5. **Glossary integration** — inline expansion for acronyms (NAS, E-UTRAN, AMF, SMF, UPF…) on hover.
6. **Diff-by-release** — link to the change-marked versions so engineers can see what actually changed between releases without scrolling 800-page documents.
7. **Search by spec number** — type `38.331` and jump straight to that document.
8. **Community contributions** — this is a static HTML site in a public repo. Pull requests welcome for corrections, new entries, and fixes to dead links.

## Contributing

The whole site is a single `index.html` driven by a small JSON-shaped data table inside it. To add or correct an entry:

1. Fork the repo.
2. Edit the `SERIES_DATA` array in the source.
3. Open a pull request with a one-line note on what changed and why.

Corrections are appreciated more than features. If a link rots or a topic description is misleading, that's the highest-leverage thing you can fix.

## License & ownership

- The **page layout, code, and curation** in this repository are released under the MIT License — fork it, host your own, modify it freely.
- The **specifications, status reports, and any document content** linked from this page are the intellectual property of **3GPP** and its Organizational Partners (ARIB, ATIS, CCSA, ETSI, TSDSI, TTA, TTC). All trademarks belong to their respective owners.

---

*Built as a path-finder, not a portal. If it saves you ten minutes the first time, it's done its job.*
