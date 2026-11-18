# RUNLU GROWTH OS — separate GitHub Pages preview

**No files in this package should be uploaded to `Runlu.ca` or merged into PR #490.** Create a NEW public repository, e.g. `runlu-growth-preview`, under `nevergiveup980-ux`.

## Deploy from iPhone / computer
1. In GitHub choose **+ → New repository**; name `runlu-growth-preview`; visibility **Public**; create with a README (optional).
2. Open that NEW repo, **Add file → Upload files**. Upload the *contents* of this ZIP to the repository root, including `index.html`, `privacy.html`, `runlu-ga4-consent.js`, `robots.txt`, `.nojekyll` and this README. Do not upload the ZIP itself as the only file. If `.nojekyll` is hidden by your phone, it is optional for this plain HTML preview.
3. In the NEW repo go to **Settings → Pages**; select **Deploy from a branch → main → /(root)**, then Save. **Do not enter a custom domain.**
4. Wait for GitHub Pages to finish. The expected URL format is `https://nevergiveup980-ux.github.io/runlu-growth-preview/` (not guaranteed live until Pages reports successful deployment).
5. Open the URL in Safari on your iPhone and follow the acceptance checks.

## Safety
- Public GitHub Pages is NOT private, even with robots.txt and noindex.
- The preview reuses GA4 measurement ID `G-KVRWEFJMCR`; accepting can send test events to production GA4. Ideally use a separate test GA4 property before network verification, or mark/exclude test traffic when reviewing results.
- The consent script is copied from PR #490's existing offline review artifact, with only its privacy-link path adapted from `/privacy.html` to `./privacy.html` for GitHub Pages project paths. The HTML wrapper is a deliberately minimal test harness, **not a full copy of the production homepage**.
- No paid products, new domain, repository secrets, CNAME, custom-domain changes, or modifications to the RUNLU main repository are needed.
- If GitHub shows a paid-plan requirement, stop rather than upgrade.
- This tests consent on a dedicated preview origin. It does not replace a final Safari check of the real homepage before merging.
