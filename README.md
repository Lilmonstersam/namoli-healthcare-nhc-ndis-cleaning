# Namoli Healthcare — NDIS Cleaning Services (Landing Page Mockup)

Static landing page mockup targeting the keyword **"ndis cleaning services"** (AU, 1,095/mo, KD 2).

## Deploy

Push to `main` on https://github.com/Lilmonstersam/namoli-healthcare-nhc-ndis-cleaning — the included GitHub Actions workflow (`.github/workflows/deploy.yml`) publishes to GitHub Pages automatically. In repo settings, set **Pages > Source** to **GitHub Actions**.

```
git init && git add . && git commit -m "NDIS cleaning landing page mockup"
git branch -M main
git remote add origin https://github.com/Lilmonstersam/namoli-healthcare-nhc-ndis-cleaning.git
git push -u origin main
```

## Notes before production

- `noindex, nofollow` meta tag is set for the mockup. Remove it when the page goes live on the real domain.
- Verify Namoli's NDIS provider registration status before publishing any "registered provider" claims. The current copy says "NDIS-screened cleaners" and "supports self-managed and plan-managed participants", which avoids claiming NDIA registration.
- Confirm current NDIS Pricing Arrangements figures if you want to publish specific hourly rates ("ndis cleaning rates" is the second highest volume query at 754/mo, so a rates table is a strong future addition).
- Hero and section images reuse existing site assets; replace with NDIS/home-cleaning imagery.
