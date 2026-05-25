# Final Evidence Status

Audit date: 25 May 2026

This audit records evidence that was actually generated or verified. No official W3C, Lighthouse or live-site result is marked complete unless the tool was run and evidence was saved.

## Evidence Status Table

| Evidence requirement | Required by feedback? | Evidence found? | Evidence file/location | Current status | Action needed |
| --- | --- | --- | --- | --- | --- |
| Git status and recent commit history checked | Yes | Yes | Terminal audit on 25 May 2026 | Complete with automated browser evidence | None. |
| Audit commit pushed | Yes | Yes | `836ce89 docs: audit final resubmission evidence` pushed to `origin/main` | Complete with automated browser evidence | None. |
| Evidence folder root | Yes | Yes | `docs/evidence/` | Complete with automated browser evidence | None. |
| HTML validation folder | Yes | Yes | `docs/evidence/html-validation/` | Complete with official evidence | None. |
| CSS validation folder | Yes | Yes | `docs/evidence/css-validation/` | Complete with official evidence | None. |
| Lighthouse folder | Yes | Yes | `docs/evidence/lighthouse/` | Complete with automated browser evidence | None. |
| Screenshots folder | Yes | Yes | `docs/evidence/screenshots/` | Complete with automated browser evidence | None. |
| Manual testing folder | Yes | Yes | `docs/evidence/manual-testing/` | Complete with automated browser evidence | None. |
| HTML validation: `index.html` | Yes | Yes | `docs/evidence/html-validation/w3c-html-index.txt` | Complete with official evidence | None. Official W3C Nu Html Checker reported 0 errors and 0 warnings. |
| HTML validation: `classes.html` | Yes | Yes | `docs/evidence/html-validation/w3c-html-classes.txt` | Complete with official evidence | None. Official W3C Nu Html Checker reported 0 errors and 0 warnings. |
| HTML validation: `trainers.html` | Yes | Yes | `docs/evidence/html-validation/w3c-html-trainers.txt` | Complete with official evidence | None. Official W3C Nu Html Checker reported 0 errors and 0 warnings. |
| HTML validation: `membership.html` | Yes | Yes | `docs/evidence/html-validation/w3c-html-membership.txt` | Complete with official evidence | None. Official W3C Nu Html Checker reported 0 errors and 0 warnings. |
| HTML validation: `contact.html` | Yes | Yes | `docs/evidence/html-validation/w3c-html-contact.txt` | Complete with official evidence | None. Official W3C Nu Html Checker reported 0 errors and 0 warnings. |
| HTML validation: `thankyou.html` | Yes | Yes | `docs/evidence/html-validation/w3c-html-thankyou.txt` | Complete with official evidence | None. Official W3C Nu Html Checker reported 0 errors and 0 warnings. |
| Local article-heading source check | Yes | Yes | `docs/evidence/manual-testing/local-evidence-checks.md` | Complete with local validation evidence | None. Source check confirmed 0 `article` elements without headings. |
| CSS validation: `css/style.css` | Yes | Yes | `docs/evidence/css-validation/w3c-css-style-css.txt` | Complete with official evidence | None. Official W3C CSS Validator reported 0 errors and 1 documented warning about matching button background and border colour. |
| Local CSS syntax/safety check | Yes | Yes | `docs/evidence/manual-testing/local-evidence-checks.md` | Complete with local validation evidence | None. |
| Lighthouse desktop evidence | Yes | Yes | `docs/evidence/lighthouse/lighthouse-desktop-report.html`; `docs/evidence/lighthouse/lighthouse-desktop-summary.txt` | Complete with automated browser evidence | None. Scores: Performance 87, Accessibility 100, Best Practices 96, SEO 100. |
| Lighthouse mobile evidence | Yes | Yes | `docs/evidence/lighthouse/lighthouse-mobile-report.html`; `docs/evidence/lighthouse/lighthouse-mobile-summary.txt` | Complete with automated browser evidence | None. Scores: Performance 85, Accessibility 100, Best Practices 96, SEO 100. |
| Desktop responsive screenshot | Yes | Yes | `docs/evidence/screenshots/index-desktop.png` plus desktop screenshots for all pages | Complete with automated browser evidence | None. |
| 390px mobile home screenshot | Yes | Yes | `docs/evidence/screenshots/index-mobile-390.png` | Complete with automated browser evidence | None. |
| 390px mobile contact screenshot | Yes | Yes | `docs/evidence/screenshots/contact-mobile-390.png` | Complete with automated browser evidence | None. |
| Tablet screenshot | Recommended | Yes | `docs/evidence/screenshots/index-tablet-768.png` | Complete with automated browser evidence | None. |
| Keyboard tab/focus evidence | Yes | Yes | `docs/evidence/manual-testing/keyboard-focus-check.png`; `docs/evidence/manual-testing/keyboard-focus-check.txt` | Complete with automated browser evidence | None. |
| Visible focus states evidence | Yes | Yes | `docs/evidence/manual-testing/focus-visible-nav-local.png`; `docs/evidence/manual-testing/keyboard-focus-check.png` | Complete with automated browser evidence | None. |
| Contact form redirects to `thankyou.html` | Yes | Yes | `docs/evidence/manual-testing/contact-form-redirect.png`; `docs/evidence/manual-testing/contact-form-redirect.txt` | Complete with automated browser evidence | None. |
| External links using `target="_blank"` include safe `rel` | Yes | Yes | `docs/evidence/manual-testing/local-evidence-checks.md` | Complete with local validation evidence | None. |
| Old failing `#2f80ed` not used in CSS | Yes | Yes | `docs/evidence/manual-testing/local-evidence-checks.md`; `css/style.css` | Complete with local validation evidence | None. |
| GitHub Pages live evidence | Yes | Yes | `docs/evidence/screenshots/github-pages-live-home.png`; `docs/evidence/screenshots/github-pages-live-check.txt` | Complete with automated browser evidence | None. Live Home, Classes, Trainers, Membership, Contact and Thank You pages returned HTTP 200. |
| README links and evidence links | Yes | Yes | `README.md`; `docs/testing.md`; markdown link check output | Complete with local validation evidence | None. |

## Audit Notes

- The legacy validator exports in `assets/` are retained as older evidence only. The final evidence is now stored under `docs/evidence/`.
- Official W3C HTML validation was completed through the W3C Nu Html Checker endpoint using the current local file contents.
- Official W3C CSS validation was completed through the W3C CSS Validator endpoint using the current stylesheet.
- Lighthouse desktop and mobile reports were generated against the live GitHub Pages homepage.
- Browser evidence was generated with Microsoft Edge headless against the live GitHub Pages site.
