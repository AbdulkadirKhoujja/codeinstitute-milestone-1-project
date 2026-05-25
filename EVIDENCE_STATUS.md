# Final Evidence Status

Audit date: 25 May 2026

This audit separates evidence already present in the repo from checks that still need official manual evidence. Local screenshots and source checks are useful supporting evidence, but they do not replace fresh W3C validation, Lighthouse, browser DevTools checks or live GitHub Pages verification.

## Evidence Status Table

| Evidence requirement | Required by feedback? | Evidence found? | Evidence file/location | Current status | Action needed |
| --- | --- | --- | --- | --- | --- |
| Git status and recent commit history checked | Yes | Yes | Terminal audit on 25 May 2026 | Complete | None. Repo started clean on `main...origin/main`; recent commits show resubmission fixes and testing docs. |
| Evidence folder root | Yes | Yes | `docs/evidence/` | Complete | None. |
| HTML validation folder | Yes | Folder added, no official evidence files yet | `docs/evidence/html-validation/readme.md` | Needs manual official evidence | Save fresh W3C Nu Html Checker exports in this folder. |
| CSS validation folder | Yes | Folder added, no official evidence file yet | `docs/evidence/css-validation/readme.md` | Needs manual official evidence | Save fresh W3C CSS Validator export in this folder. |
| Lighthouse folder | Yes | Folder added, no official evidence files yet | `docs/evidence/lighthouse/readme.md` | Needs manual official evidence | Save desktop and mobile Lighthouse evidence in this folder. |
| Screenshots folder | Yes | Yes | `docs/evidence/screenshots/` | Complete | None for local screenshot support. |
| Manual testing folder | Yes | Yes | `docs/evidence/manual-testing/focus-visible-nav-local.png`; `docs/evidence/manual-testing/local-evidence-checks.md` | Complete locally, official check still recommended | Complete final hands-on keyboard and form checks in browser before contacting the lecturer. |
| HTML validation: `index.html` | Yes | Yes, but old/unclear | `assets/html-validator-index.html` | Needs replacement because old/unclear | Re-run official W3C Nu Html Checker after the article-heading fix and save fresh evidence. |
| HTML validation: `classes.html` | Yes | Yes, but stored as legacy asset | `assets/html-validator-classes.html` | Needs manual official evidence | Re-run official W3C Nu Html Checker against the current file and save fresh evidence. |
| HTML validation: `trainers.html` | Yes | Yes, but old/unclear | `assets/html-validator-trainers.html` | Needs replacement because old/unclear | Re-run official W3C Nu Html Checker after the article-heading fix and save fresh evidence. |
| HTML validation: `membership.html` | Yes | Yes, but stored as legacy asset | `assets/html-validator-membership.html` | Needs manual official evidence | Re-run official W3C Nu Html Checker against the current file and save fresh evidence. |
| HTML validation: `contact.html` | Yes | Yes, but stored as legacy asset | `assets/html-validator-contact.html` | Needs manual official evidence | Re-run official W3C Nu Html Checker against the current file and save fresh evidence. |
| HTML validation: `thankyou.html` | Yes | No | No saved W3C export found | Missing | Run official W3C Nu Html Checker and save fresh evidence. |
| Local article-heading source check | Yes | Yes | Local audit command output; `index.html`; `trainers.html` | Complete locally, official check still recommended | Official W3C replacement still needed for final evidence. |
| CSS validation: `css/style.css` | Yes | Yes, but old/unclear | `assets/w3c-css-validator-style-css.html` | Needs replacement because old/unclear | Re-run official W3C CSS Validator because the saved export still shows the old deprecated `clip` warning. |
| Local CSS syntax/safety check | Yes | Yes | Local audit command output; `css/style.css` | Complete locally, official check still recommended | Official CSS Validator replacement still needed. |
| Lighthouse desktop evidence | Yes | No | No desktop Lighthouse report or screenshot found | Missing | Run Lighthouse desktop on the live GitHub Pages site and save evidence. |
| Lighthouse mobile evidence | Yes | No | No mobile Lighthouse report or screenshot found | Missing | Run Lighthouse mobile on the live GitHub Pages site and save evidence. |
| Desktop responsive screenshot | Yes | Yes | `docs/evidence/screenshots/index-desktop.png` plus desktop screenshots for all pages | Complete | None for local desktop screenshot support. |
| 390px mobile home screenshot | Yes | Yes | `docs/evidence/screenshots/index-mobile-390.png` | Complete locally, official check still recommended | Also confirm in browser DevTools if the lecturer expects manual DevTools evidence. |
| 390px mobile contact screenshot | Yes | Yes | `docs/evidence/screenshots/contact-mobile-390.png` | Complete locally, official check still recommended | Also confirm in browser DevTools if the lecturer expects manual DevTools evidence. |
| Tablet screenshot | Recommended | Yes | `docs/evidence/screenshots/index-tablet-768.png` | Complete locally, official check still recommended | None unless broader tablet page evidence is requested. |
| Keyboard tab/focus evidence | Yes | Partial | `docs/evidence/manual-testing/focus-visible-nav-local.png`; `css/style.css` | Complete locally, official check still recommended | Manually tab through the live/local site and save a short note or screenshot if required. |
| Visible focus states evidence | Yes | Yes, local | `docs/evidence/manual-testing/focus-visible-nav-local.png`; `css/style.css` | Complete locally, official check still recommended | Manual browser confirmation still recommended. |
| Contact form redirects to `thankyou.html` | Yes | Partial | `contact.html`; `docs/evidence/screenshots/thankyou-desktop.png`; `docs/evidence/manual-testing/local-evidence-checks.md` | Complete locally, official check still recommended | Submit the form manually in a browser and save evidence if required. |
| External links using `target="_blank"` include safe `rel` | Yes | Yes | Local audit command output; all HTML footers | Complete | None. |
| Old failing `#2f80ed` not used in CSS | Yes | Yes | Local audit command output; `css/style.css` | Complete | None. |
| GitHub Pages live evidence | Yes | README has URL only | `README.md` | Needs manual official evidence | After pushing, open the live GitHub Pages site and save evidence. |
| README links and evidence links | Yes | Yes, updated | `README.md`; `docs/testing.md` | Complete locally, official check still recommended | Re-check after adding final manual evidence files. |

## Audit Notes

- Existing W3C HTML exports for `index.html` and `trainers.html` are not final evidence because they still show article-heading warnings that the source code has since been fixed for.
- Existing CSS validator evidence is not final evidence because it still records the old deprecated `clip` warning, while the current stylesheet uses `clip-path: inset(50%)`.
- No Lighthouse evidence was found.
- Local Edge screenshots were added on 25 May 2026 for 390px home, 390px contact, tablet home and visible focus support.
