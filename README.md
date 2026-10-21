# DayAtlas entry policies

Public, reviewed reference data for DayAtlas. The app verifies the signed manifest and exact catalog bytes before accepting updates.

The initial coverage is a small curated set, not a worldwide eligibility service. Entry conditions and source/review dates are included in the catalog. Individual immigration decisions, issued permissions and actual admission periods remain separate.

No personal passports, permits, trips, locations, accounts, private signing material or client tokens belong in this repository.

`v1/head.json` selects an immutable signed-catalog payload in `v1/catalogs/`. Historical rule revisions remain in each full catalog. Ordinary data updates are independent of the app release cycle.

Sequence 3 adds reviewed short-tourism references for ordinary China passports visiting Qatar, Oman, Thailand and Malaysia. These are qualified entry/stay references, with official source links and conditions; they do not calculate a personal grant or remaining legal allowance. Earlier revisions are preserved. Source review and validation are tracked in [DayAtlas issue 307](https://github.com/akirakusen/dayatlas/issues/307).

Sequence 4 adds reviewed Nepal and Maldives references for ordinary China passports and updates Indonesia's arrival-visa reference to 30 days. Nepal's initial duration choices remain distinct from its annual cap; Maldives follows the bilateral visa exemption. All are qualified references without personal admission grants or executable stay limits. See [DayAtlas issue 309](https://github.com/akirakusen/dayatlas/issues/309).

Sequence 5 adds the short-tourism Schengen visa requirement for ordinary China passports, including France. Existing visas and qualifying residence documents remain separate personal entry options. The reference has no stated duration or executable limits, and the general 90/180-day ceiling is not an individual visa grant. Earlier catalog bytes and records are preserved. See [DayAtlas issue 315](https://github.com/akirakusen/dayatlas/issues/315).
