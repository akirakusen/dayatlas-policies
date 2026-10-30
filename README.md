# DayAtlas entry policies

Public reference data for DayAtlas. The app verifies the signed manifest and exact catalog bytes before accepting an update. No personal passports, permits, trips, locations, accounts, private signing material or client tokens belong in this repository.

`v1/head.json` selects an immutable signed catalog in `v1/catalogs/`. Historical revisions remain in every full catalog. Ordinary data updates are independent of app releases.

Catalog 6 introduced source-specific official Schengen, UK and Japan nationality groups with a **dated third-party ordinary-tourism summary**. The aggregate is VisaMundial version 2026.2, dated **6 August 2026**; local intake on 21 October does not establish current government accuracy for every pair. [Credits and full licenses](ATTRIBUTION.md) identify source attribution, modifications, CC BY 4.0 and the upstream MIT notice.

Legacy catalog 7 and capable catalog 8 preserve the complete history and reconcile Sri Lanka tourism with its official ETA notice effective 25 May 2026. All 197 foreign ordinary-passport issuer scopes have reviewed references; free ETA processing is distinct from exemption. The HKSAR source conflict remains conditional, and GB nationality subclasses receive no automatic free-processing or duration claim. The [Sri Lanka ETA authority](https://eta.gov.lk/slvisa/) and [exemptions table](https://www.eta.gov.lk/slvisa/visainfo/diplo.jsp?locale=en_US) are retained as dated sources. No duration becomes an executable visitor allowance.

Legacy catalog 9 and capable catalog 10 renew the two China–Singapore ordinary-passport tourism references from the [Chinese Embassy in Singapore](https://sg.china-embassy.gov.cn/eng/lsfwx/va/zgqz/202609/t20260918_12025190.htm) and the [NIA bilateral table](https://en.nia.gov.cn/n147418/n147463/c181470/content.html). Both retain a 30-day reference and unconfirmed general entry requirements; the Singapore-to-China reference removes an unsupported generic cumulative note. Personal permissions and actual admissions remain separate. Other dated references keep their existing review scope. [Publication tracking](https://github.com/akirakusen/dayatlas-policies/issues/8).

Capable catalog 11 renews the Malaysia ordinary-visitor references for China and Singapore passports, reviewed on 29 October 2026 through 8 November inclusive. China retains 30 days per entry and the qualified 90-in-180 condition from the [Immigration FAQ](https://www.imi.gov.my/wp-content/uploads/2022/01/21OKT_FAQs-MYS-CHINA_LULUS.pdf); the existing uncertainty about that period remains. Singapore retains a 30-day reference with the entry-stamp qualification. Personal documents and actual admissions remain separate. This capability-bearing update leaves legacy catalog 9 unchanged for older readers; it does not activate the wider Malaysia nationality matrix. [Publication tracking](https://github.com/akirakusen/dayatlas-policies/issues/10).

Current capable catalog 13 combines 34 destination scopes, including Thailand, Taiwan, Indonesia and Vietnam, with supporting-document alternatives and Türkiye entry-document terms. It preserves every historical definition and the latest Malaysia and China–Singapore successors. The graph contains 206 sources, 743 ordinary policy objects (658 selected), 28 selected alternatives and one Türkiye document rule. The unchanged legacy feed remains catalog 9. [Publication tracking](https://github.com/akirakusen/dayatlas-policies/issues/12).

Original review dates and conditional branches remain explicit. Several document scopes are due for review on 31 October or 1 November; ordinary 23–24 October reviews are due 2–3 November. August aggregate residuals retain their original dates. This is not a fresh government review of every passport/destination pair. Published stay references do not prove visa ownership, admission or an individual permitted stay; applicable personal documents and actual grants remain separate.

Conversion, coverage and verification are tracked in [DayAtlas issue 320](https://github.com/akirakusen/dayatlas/issues/320).

## Compatible reader bases

The root base remains the legacy feed for existing DayAtlas releases. `feeds/entry-alternatives-v1/` is a separate base for compatible releases that understand its required capabilities. Both bases reuse the signed `v1/head.json` and immutable `v1/catalogs/...` format, the same trust key and the same feed identity. A new app base does not bypass sequence, capability, signature or continuity checks.

The compatible base starts with byte-identical signed catalog 6 and its payload. This bootstrap adds no rules, changes no legacy bytes and creates no new signature. Later capability-bearing updates belong only in the compatible base; ordinary reference updates must continue to maintain the legacy base as well. Never overwrite an immutable catalog.

Existing apps do not discover another base automatically. App activation follows published-byte verification and a compatible reader update, tracked in [DayAtlas issue 373](https://github.com/akirakusen/dayatlas/issues/373). This bootstrap is tracked in [policy issue 5](https://github.com/akirakusen/dayatlas-policies/issues/5).
