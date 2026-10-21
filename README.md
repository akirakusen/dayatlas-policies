# DayAtlas entry policies

Public reference data for DayAtlas. The app verifies the signed manifest and exact catalog bytes before accepting an update. No personal passports, permits, trips, locations, accounts, private signing material or client tokens belong in this repository.

`v1/head.json` selects an immutable signed catalog in `v1/catalogs/`. Historical revisions remain in every full catalog. Ordinary data updates are independent of app releases.

Catalog 6 combines source-specific official Schengen, UK and Japan nationality groups with a **dated third-party ordinary-tourism summary**. The aggregate is VisaMundial version 2026.2, dated **6 August 2026**; local intake on 21 October does not establish current government accuracy for every pair. [Credits and full licenses](ATTRIBUTION.md) identify source attribution, modifications, CC BY 4.0 and the upstream MIT notice.

There are 39,037 supported reference pairs, including 32,890 dated aggregate references. Aggregate records have no stated duration or executable allowance. Special passport documents, individual status, itinerary conditions, 51 territory destinations and missing self combinations may remain unresolved. Current official scope corrections take priority; a summary is not proof of admission, visa ownership or a permitted stay. Personal documents and grants remain separate.

Conversion, coverage and verification are tracked in [DayAtlas issue 320](https://github.com/akirakusen/dayatlas/issues/320).
