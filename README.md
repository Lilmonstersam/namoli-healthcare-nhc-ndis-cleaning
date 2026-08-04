# Namoli Healthcare — Care Centre & Respite Cleaning (Landing Page Mockup)

Static landing page mockup for multi-site care centre operators (BlueCare / AusCare type organisations).

**Audience: care centre operators, not individuals and not individual accommodation.** Scope is residential care centres, including dementia and memory support wings, plus respite and day centres. Domestic cleaning and individual disability accommodation (SIL/SDA/group homes) are explicitly out of scope.

## Keyword basis (Ahrefs, AU)

| Keyword | Vol/mo | KD | Role on page |
|---|---|---|---|
| aged care cleaning | 338 | 0 | Primary cluster (TP 1,000) |
| aged care cleaning services | 270 | 0 | Primary cluster (TP 1,000) |
| aged care cleaning melbourne / brisbane | 109 / 101 | 0 | Geo signals |
| aged care facility cleaning | 40 | - | Supporting |
| surface cleaning in aged care | 108 | 0 | Informational coverage (ATP/testing section) |
| environment cleaning in aged care | 101 | - | Informational coverage (standards section) |
| nursing home cleaning services | 30 | - | Supporting |
| ndis cleaning services | 1,095 | 2 | Not targeted; see note |

**Positioning vs search volume, read this before judging the page on rankings.** The title and H1 now lead with "care centre" and "respite centre", which are the terms the client uses but which carry very little search volume in Australia. "Respite care cleaning" and "dementia care cleaning" return effectively no data in Ahrefs. The searchable demand for this offer sits in the **aged care cleaning** cluster (338 + 270/mo, KD 0, TP 1,000), which the body copy, FAQs and schema now support but the title tag does not.

Two consequences worth a decision:

1. If organic traffic matters for this page, the title and H1 should carry "aged care cleaning" somewhere, e.g. "Aged Care & Respite Centre Cleaning Services". As written, the page is optimised for how the client talks rather than how buyers search.
2. **"NDIS cleaning services" (1,095/mo) is no longer targeted.** It was the original brief's primary keyword, but with SIL/SDA and domestic cleaning out of scope there is no NDIS-funded service left to rank for. NDIS is now referenced only where centres deliver disability respite. If that volume is still wanted, it needs a separate page and a service Namoli actually sells.

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
- Repo and folder are still named `namoli-healthcare-nhc-ndis-cleaning`, which no longer matches the page. Rename before this becomes the live URL slug.
- Consider whether "NDIS cleaning services" (1,095/mo) is worth a separate page tied to a service Namoli genuinely sells, rather than leaving that demand unaddressed.
