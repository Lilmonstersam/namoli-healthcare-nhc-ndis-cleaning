# Namoli Healthcare — NDIS Cleaning for Care & Respite Centres (Landing Page Mockup)

Static landing page mockup. Primary keyword: **"ndis cleaning"** / **"ndis cleaning services"** (AU, 722 + 1,095/mo, KD 2).

**Audience: NDIS care centre and respite centre operators, including multi-site organisations (BlueCare / AusCare type).** Scope is NDIS care centres, residential care centres including dementia and memory support wings, and respite and day centres. Domestic cleaning in participants' private homes and individual accommodation (SIL/SDA/group homes) are out of scope.

## Keyword basis (Ahrefs, AU)

| Keyword | Vol/mo | KD | Role on page |
|---|---|---|---|
| ndis cleaning services | 1,095 | 2 | Title / H1 (primary) |
| ndis cleaning | 722 | 2 | Primary, body copy |
| ndis cleaners | 242 | 7 | Supporting |
| aged care cleaning | 338 | 0 | Secondary cluster (TP 1,000) |
| aged care cleaning services | 270 | 0 | Secondary cluster (TP 1,000) |
| aged care cleaning melbourne / brisbane | 109 / 101 | 0 | Geo signals |
| surface cleaning in aged care | 108 | 0 | Informational coverage (ATP/testing section) |
| environment cleaning in aged care | 101 | - | Informational coverage (standards section) |

**Intent management is the whole job on this page.** The NDIS cleaning SERP skews participant-side: people searching for domestic help funded through Household Tasks. Ranking is easy at KD 2, but a large share of that traffic is individuals Namoli cannot serve. Rather than chase or ignore it, the page qualifies hard and early:

- Title and meta description both say "care centres and respite centres, not private homes", so the wrong audience self-selects out at the SERP before costing a click.
- H1 pairs the keyword with the qualifier: "NDIS Cleaning Services for Care & Respite Centres".
- A visible note directly under the hero intro states that Namoli cleans centres operated by care providers, not participants' private homes.
- A dedicated FAQ repeats the boundary and redirects participants to their support coordinator or plan manager.

Expect a below-average CTR on this keyword as a result. That is intentional: the clicks that remain are operators, not participants. Watch enquiry quality rather than raw traffic when judging the page.

"Respite care cleaning", "dementia care cleaning" and "SIL cleaning services" have effectively no search volume in Australia, so they serve as on-page service coverage and conversion copy, not keyword targets. The aged care cluster (KD 0, TP 1,000) is supported through body copy, FAQs and schema and is the natural second page if this one performs.

## Deploy

Push to `main` on https://github.com/Lilmonstersam/namoli-healthcare-nhc-ndis-cleaning — the workflow at `.github/workflows/deploy.yml` publishes to GitHub Pages. In repo settings, set **Pages > Source** to **GitHub Actions**.

```
git add . && git commit -m "Pivot copy to care facilities"
git push
```

## Notes before production

- `noindex, nofollow` meta tag is set for the mockup. Remove it when the page goes live on the real domain.
- Verify Namoli's NDIS provider registration status before publishing any NDIS-related claims. Current copy says "NDIS Worker Screening Check" and references the NDIS Practice Standards only where centres deliver disability respite, which avoids claiming NDIA registration.
- Confirm the ATP testing, 3M protein pen and monthly audit claims apply to residential care and respite contracts, not just clinical sites.
- **Verify the multi-site claims.** The portfolio FAQ and the "Consistent Across Every Site" bullet promise a single account manager, one reporting format, a named supervisor per centre and group-level audit roll-up. This is the strongest differentiator against a single-site cleaner and the exact thing a large operator will probe, so it must be operationally true before it goes live.
- Standards are referenced by name only (Aged Care Quality Standards, NDIS Practice Standards) with no clause numbers, since the strengthened aged care standards renumbered requirements. Add specifics only once verified.
- "Three-Win Philosophy" and TreeLabs claims carried over from existing brand material; confirm still current.
- Repo and folder name `namoli-healthcare-nhc-ndis-cleaning` matches the page again, so no rename needed.
- Consider a follow-up page on the "aged care cleaning services" cluster (KD 0, TP 1,000) so NDIS and aged care demand are not competing for one URL.
