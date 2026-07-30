# Namoli Healthcare — NDIS Cleaning Services (Landing Page Mockup)

Static landing page mockup. Primary keyword: **"ndis cleaning services"** (AU, 1,095/mo, KD 2).

**Audience: care providers, not individual participants.** Namoli does not do domestic cleaning, so the page targets facility decision makers in residential aged care, NDIS disability accommodation (SIL/SDA/group homes), dementia and memory support units, and respite and day centres.

## Keyword basis (Ahrefs, AU)

| Keyword | Vol/mo | KD | Role on page |
|---|---|---|---|
| ndis cleaning services | 1,095 | 2 | H1 / title (primary) |
| ndis cleaning | 722 | 2 | Supporting, body copy |
| aged care cleaning | 338 | 0 | Secondary cluster (TP 1,000) |
| aged care cleaning services | 270 | 0 | Secondary cluster (TP 1,000) |
| disability cleaning services | 113 | 1 | Disability-side variant |
| aged care cleaning melbourne / brisbane | 109 / 101 | 0 | Geo signals |
| surface cleaning in aged care | 108 | 0 | Informational coverage (ATP/testing section) |
| environment cleaning in aged care | 101 | - | Informational coverage (standards section) |

**Intent note:** the "ndis cleaning" SERP skews participant-side (Household Tasks funding, hourly rates). Ranking for it is easy (KD 2) but a share of that traffic will be individuals seeking domestic cleaning. The page handles this deliberately with an FAQ that states Namoli is facility-only, which protects lead quality. "Dementia care cleaning", "respite care cleaning" and "SIL cleaning services" have effectively no search volume in Australia, so they are used as on-page service coverage and conversion copy rather than keyword targets.

## Deploy

Push to `main` on https://github.com/Lilmonstersam/namoli-healthcare-nhc-ndis-cleaning — the workflow at `.github/workflows/deploy.yml` publishes to GitHub Pages. In repo settings, set **Pages > Source** to **GitHub Actions**.

```
git add . && git commit -m "Pivot copy to care facilities"
git push
```

## Notes before production

- `noindex, nofollow` meta tag is set for the mockup. Remove it when the page goes live on the real domain.
- Verify Namoli's NDIS provider registration status before publishing any "registered provider" claims. Current copy says "NDIS Worker Screening Check" and "supports your obligations under the NDIS Practice Standards", which avoids claiming NDIA registration.
- Confirm the ATP testing, 3M protein pen and monthly audit claims apply to aged care and disability contracts, not just clinical sites.
- Standards are referenced by name only (NDIS Practice Standards, Aged Care Quality Standards) with no clause numbers, since the strengthened aged care standards renumbered requirements. Add specifics only once verified.
- **Confirm whether Namoli actually services SIL, SDA and group homes.** Not yet verified with the client. The copy is written as capability rather than an existing client base, and scopes the work as provider-contracted cleaning of shared and communal areas. If Namoli does not service this segment at all, the SIL/SDA card and FAQ should come out, and the page should be re-targeted to "aged care cleaning services" (KD 0, TP 1,000), because the NDIS angle depends on this segment.
- Scope boundary to reflect in any proposal: shared and communal areas, periodic deep cleans, carpets, windows and vacancy turnovers sit with the provider contract. A resident's personal bedroom is often covered by support workers or the participant's own plan, so it is scoped separately by agreement.
- "Three-Win Philosophy" and TreeLabs claims carried over from existing brand material; confirm still current.
- Consider a follow-up page targeting the pure "aged care cleaning services" cluster (KD 0, TP 1,000) so the NDIS and aged care demand is not competing for one URL.
