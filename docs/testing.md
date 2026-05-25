# Testing and Resubmission Evidence

Testing date: 10 May 2026

This file records the checks completed during the resubmission preparation and the manual checks still required before final submission. Results are not invented: where this environment cannot run an official browser audit, W3C validator check or Lighthouse report, the row is marked as manual follow-up.

Final evidence audit files:

* [Resubmission checklist](../RESUBMISSION_CHECKLIST.md)
* [Final evidence status](../EVIDENCE_STATUS.md)
* [Final manual evidence steps](../FINAL_MANUAL_STEPS.md)
* [Evidence folder](evidence/)

## Manual Testing Matrix

| Page or area | Test action | Expected result | Actual result | Status | Date |
| --- | --- | --- | --- | --- | --- |
| `index.html` | Open the home page and use the main navigation links. | Navigation links load Home, Classes, Trainers, Membership and Contact pages. | To be completed manually in browser before submission. | Manual follow-up | 10 May 2026 |
| `classes.html` | Review class cards and weekly timetable. | Class information is readable and timetable remains usable. | Desktop and narrow screenshots generated successfully. | Pass - screenshot evidence | 10 May 2026 |
| `trainers.html` | Review trainer cards and testimonial section. | Trainer cards have headings; testimonial cards no longer trigger article-heading warnings. | Source updated from quote-only `article` cards to `div.card`. | Pass - code check | 10 May 2026 |
| `membership.html` | Review plan cards and call-to-action links. | Plans are readable and Join Now links go to Contact. | Desktop and narrow screenshots generated successfully. | Pass - screenshot evidence | 10 May 2026 |
| `contact.html` | Complete required form fields and submit. | Form redirects to `thankyou.html`. | Form action is `thankyou.html`; full browser submission to be repeated manually. | Manual follow-up | 10 May 2026 |
| `thankyou.html` | Open after form submission or direct URL. | Confirmation message and next-step links display. | Desktop and narrow screenshots generated successfully. | Pass - screenshot evidence | 10 May 2026 |
| Internal links | Inspect internal page links and navigation hrefs. | Internal links point to existing local HTML files. | Source inspection completed; no missing internal page targets found. | Pass - code check | 10 May 2026 |
| External links | Search for social links using `target="_blank"`. | Every new-tab external link includes `rel="noopener noreferrer"`. | `rg "target"` confirmed all social links include the security attributes. | Pass - code check | 10 May 2026 |
| Responsive layout | Capture desktop and narrow screenshots. | Content remains readable and layouts collapse appropriately. | Screenshots generated in `docs/evidence/screenshots/`. | Pass - screenshot evidence | 10 May 2026 |
| 390px mobile layout | Capture home and contact at 390px width. | No horizontal scrolling, text clipping or overlapping content is visible in the captured viewport. | Local Edge screenshots added: `index-mobile-390.png` and `contact-mobile-390.png`; manual DevTools confirmation is still recommended. | Pass - local screenshot evidence | 25 May 2026 |
| Tablet layout | Capture home page at tablet width. | Layout remains readable at tablet width. | Local Edge screenshot added: `index-tablet-768.png`. | Pass - local screenshot evidence | 25 May 2026 |
| Keyboard navigation | Tab through header, buttons, links and form controls. | Focus order is logical and every focused item has a visible indicator. | `:focus-visible` styles added and one local focused-nav screenshot captured; full browser tab-through still needs manual confirmation. | Manual follow-up | 25 May 2026 |
| Visible focus states | Check nav links, buttons, form controls and footer links. | Focus styles are clear on light and dark backgrounds. | `focus-visible-nav-local.png` shows the Classes nav link focused; manual visual check across all controls remains recommended. | Pass - local evidence | 25 May 2026 |
| Colour contrast | Compare old and new button/nav/link colours. | Normal interactive text meets at least 4.5:1 contrast. | `#005ea8` on white is 6.63:1; `#004b8d` on white is 8.78:1. | Pass - contrast check | 10 May 2026 |
| HTML validation | Validate each HTML file using W3C Nu Html Checker. | No errors or warnings after fixes. | Existing saved exports are old for `index.html` and `trainers.html`; fresh validation must be run manually. | Manual follow-up | 10 May 2026 |
| CSS validation | Validate `css/style.css` using W3C CSS Validator. | No errors; any warnings documented. | Deprecated `clip` warning fixed; fresh official CSS validation must be run manually. | Manual follow-up | 10 May 2026 |
| Lighthouse | Run Lighthouse for performance, accessibility, best practices and SEO. | Scores and findings are recorded with screenshot evidence. | Lighthouse is not installed locally in this environment. | Manual follow-up | 10 May 2026 |
| GitHub Pages deployment | Open the deployed GitHub Pages URL after pushing. | Live site reflects the final committed source. | To be completed after final push. | Manual follow-up | 10 May 2026 |

## Screenshot Evidence

Desktop and narrow viewport screenshots were produced with Microsoft Edge headless and saved in `docs/evidence/screenshots/`.

| Page | Desktop file | Narrow file |
| --- | --- | --- |
| Home | `index-desktop.png` | `index-narrow.png` |
| Classes | `classes-desktop.png` | `classes-narrow.png` |
| Trainers | `trainers-desktop.png` | `trainers-narrow.png` |
| Membership | `membership-desktop.png` | `membership-narrow.png` |
| Contact | `contact-desktop.png` | `contact-narrow.png` |
| Thank You | `thankyou-desktop.png` | `thankyou-narrow.png` |

Additional evidence generated on 25 May 2026:

| Check | File |
| --- | --- |
| Home at 390px | `index-mobile-390.png` |
| Contact at 390px | `contact-mobile-390.png` |
| Home at 768px tablet width | `index-tablet-768.png` |
| Focus-visible navigation state | `evidence/manual-testing/focus-visible-nav-local.png` |
| Local source/link/form checks | `evidence/manual-testing/local-evidence-checks.md` |

## Local Static Checks Run

The following local checks were run during the resubmission work:

| Check | Command or method | Result |
| --- | --- | --- |
| Old inaccessible blue removed from stylesheet | `rg -n "#2f80ed|#1366d6|clip:|:focus" css/style.css` | Only intentional `:focus-visible` selectors remain; old colour values and deprecated `clip:` are absent from CSS. |
| External-link security attributes | `rg -n "target" .` | All external social links using `target="_blank"` include `rel="noopener noreferrer"`. |
| Evidence filename scan | PowerShell scan for capitals, spaces, ampersands, brackets and underscores in `assets/` filenames | No non-compliant evidence filenames found. |
| Screenshot generation | Microsoft Edge headless screenshots for all pages | Desktop and narrow screenshots generated successfully in `docs/evidence/screenshots/`. |
| Contrast calculation | Relative luminance calculation for old and new blues | Old `#2f80ed` on white: 3.87:1; new `#005ea8` on white: 6.63:1; hover `#004b8d` on white: 8.78:1. |

## Validation Follow-Up Instructions

Before final resubmission:

1. Open https://validator.w3.org/nu/.
2. Validate `index.html`, `classes.html`, `trainers.html`, `membership.html`, `contact.html` and `thankyou.html`.
3. Save each result into `docs/evidence/html-validation/` using lower-case hyphenated filenames, for example `html-validation-thankyou.html`.
4. Treat the old `assets/` validator exports as legacy evidence only after the fresh post-fix exports are saved.
5. Open https://jigsaw.w3.org/css-validator/.
6. Validate `css/style.css` and save the updated result as `docs/evidence/css-validation/css-validation-style-css.html`.
7. If the CSS validator reports a warning about matching button background and border colours, document it as harmless because the solid button design intentionally uses the same colour for fill and border.

## Lighthouse Follow-Up Instructions

Before final resubmission:

1. Open the deployed GitHub Pages URL in Chrome or Edge.
2. Open DevTools and run Lighthouse for mobile and desktop.
3. Save screenshots or exported reports in `docs/evidence/lighthouse/`.
4. Add the scores and any actions taken to this file.

## Bugs and Fixes

| Bug or risk | Fix applied | Evidence |
| --- | --- | --- |
| Failed interactive colour contrast. | Replaced `#2f80ed` with `#005ea8` and hover `#004b8d`. | README accessibility table and `css/style.css`. |
| Inconsistent keyboard focus visibility. | Added `:focus-visible` styles and stronger focus rings. | `css/style.css`. |
| HTML validator article-heading warnings. | Changed quote-only testimonial cards from `article` to `div`. | `index.html`, `trainers.html`. |
| Missing external-link security attributes. | Added `rel="noopener noreferrer"` to `contact.html` social links and verified all files. | `contact.html` and `rg "target"` check. |
| Evidence filenames were not maintainable. | Renamed evidence files to lower-case hyphenated names. | `assets/`. |
