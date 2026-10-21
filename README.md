# DayAtlas entry policies

Public reference data for DayAtlas. The app verifies the signed manifest and exact catalog bytes before accepting an update. No personal passports, permits, trips, locations, accounts, private signing material or client tokens belong in this repository.

`v1/head.json` selects an immutable signed catalog in `v1/catalogs/`. Historical revisions remain in every full catalog. Ordinary data updates are independent of app releases.

Catalog 6 combines source-specific official Schengen, UK and Japan nationality groups with a **dated third-party ordinary-tourism summary**. The aggregate is VisaMundial version 2026.2, dated **6 August 2026**; local intake on 21 October does not establish current government accuracy for every pair. [Credits and full licenses](ATTRIBUTION.md) identify source attribution, modifications, CC BY 4.0 and the upstream MIT notice.

There are 39,037 supported reference pairs, including 32,890 dated aggregate references. Aggregate records have no stated duration or executable allowance. Special passport documents, individual status, itinerary conditions, 51 territory destinations and missing self combinations may remain unresolved. Current official scope corrections take priority; a summary is not proof of admission, visa ownership or a permitted stay. Personal documents and grants remain separate.

Conversion, coverage and verification are tracked in [DayAtlas issue 320](https://github.com/akirakusen/dayatlas/issues/320).

## Compatible reader bases

The root base remains the legacy feed for existing DayAtlas releases. `feeds/entry-alternatives-v1/` is a separate base for a future reader that understands `entry-alternatives-v1`. Both bases reuse the signed `v1/head.json` and immutable `v1/catalogs/...` format, the same trust key and the same feed identity. A new app base does not bypass sequence, capability, signature or continuity checks.

The compatible base starts with byte-identical signed catalog 6 and its payload. This bootstrap adds no rules, changes no legacy bytes and creates no new signature. Later capability-bearing updates belong only in the compatible base; ordinary reference updates must continue to maintain the legacy base as well. Never overwrite an immutable catalog.

Existing apps do not discover another base automatically. App activation follows published-byte verification and a compatible reader update, tracked in [DayAtlas issue 373](https://github.com/akirakusen/dayatlas/issues/373). This bootstrap is tracked in [policy issue 5](https://github.com/akirakusen/dayatlas-policies/issues/5).
