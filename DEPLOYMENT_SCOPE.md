# STG Digital Tanzania — deployment scope and recovery status

**Date:** 22 October 2026  
**Branch:** `stg-integrated-ux-feedback-20261022`  
**Purpose:** User-experience and navigation feedback only — no clinical prescribing.

## What is hosted here
- `overview.html`: interactive responsive integrated-platform navigation preview.
- `review/index.html`: previous limited V17 medicine demonstration, not an independently approved clinical reference.
- `index.html`: redirects to the integrated overview.
- Feedback action opens a GitHub issue draft. No patient or identifying health information should be entered.

## What exists only in recovered local source
The user-provided 22 October Next.js source contains STG, Diseases, Medicines, Treat, Calculator, Departments, Learn, Search, Sources, Reader, Saved, and Settings. Recovery also incorporated compatible V20 clinical-review dossiers and PostgreSQL governance SQL, **not** working V20 staff routes.

- 89 / 89 available Node regression tests pass after replacing an absolute test-fixture path with a bundled portable reader fixture.
- National STG SHA-256 check passes; 2,800 indexed source pages across 6 volumes and 1,734 base index entries.
- Next.js `npm install`, semantic typecheck, `next build`, browser E2E and PostgreSQL authentication/integration tests are **not yet verified**.
- Full source is **not committed here** because content redistribution and rights-filtering are unresolved, and this repository is public.
- 751 indexed medicine entries must not be described as 751 independently reviewed monographs.
- Calculators and prescribing modules must stay disabled to the public until verified patient eligibility and medication dosing rules, clinical sign-off, privacy controls and publication rights are complete.

## Production
The default `main` branch is intentionally unchanged. The Vercel deployment generated from this branch targets **preview**, not **production**. Do not relabel this static UX demo as the full Next.js V20 application.
