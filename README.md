# DayAtlas entry policies

Public, reviewed reference data for DayAtlas. The app verifies the signed manifest and exact catalog bytes before accepting updates.

The initial coverage is a small curated set, not a worldwide eligibility service. Entry conditions and source/review dates are included in the catalog. Individual immigration decisions, issued permissions and actual admission periods remain separate.

No personal passports, permits, trips, locations, accounts, private signing material or client tokens belong in this repository.

`v1/head.json` selects an immutable signed-catalog payload in `v1/catalogs/`. Historical rule revisions remain in each full catalog. Ordinary data updates are independent of the app release cycle.

Sequence 3 adds reviewed short-tourism references for ordinary China passports visiting Qatar, Oman, Thailand and Malaysia. These are qualified entry/stay references, with official source links and conditions; they do not calculate a personal grant or remaining legal allowance. Earlier revisions are preserved. Source review and validation are tracked in [DayAtlas issue 307](https://github.com/akirakusen/dayatlas/issues/307).
