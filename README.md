# CommunityFit Gym Website

CommunityFit Gym is a static HTML and CSS website created for the Code Institute User-Centric Frontend Development Milestone Project. The project presents a welcoming local gym with clear information about classes, trainers, membership options, opening hours and contact routes.

Live site: https://abdulkadirkhoujja.github.io/codeinstitute-milestone-1-project/

## Project Purpose

The site is designed to help potential and current gym members quickly understand what CommunityFit Gym offers. The project focuses on accessible navigation, readable content, friendly visual design and responsive layouts across desktop and smaller screens.

## Target Users

* People considering joining a local gym.
* Beginners who want a welcoming and non-intimidating fitness environment.
* Existing members checking classes, opening hours or contact details.
* Users who need a simple contact form and clear gym information.

## User Stories

| User story | How the site meets it | Evidence |
| --- | --- | --- |
| As a new visitor, I want to understand the gym atmosphere quickly. | The home page hero and benefit cards explain the friendly community focus. | [Home desktop screenshot](docs/evidence/screenshots/index-desktop.png) |
| As a beginner, I want to find approachable classes. | The classes page lists class types, levels and a weekly timetable. | [Classes desktop screenshot](docs/evidence/screenshots/classes-desktop.png) |
| As a potential member, I want to compare membership options. | The membership page shows three plan cards and benefits. | [Membership desktop screenshot](docs/evidence/screenshots/membership-desktop.png) |
| As a user choosing support, I want to learn about trainers. | The trainers page introduces trainer profiles and coaching approach. | [Trainers desktop screenshot](docs/evidence/screenshots/trainers-desktop.png) |
| As a user with a question, I want to contact the gym easily. | The contact page includes contact details, opening hours and a form. | [Contact desktop screenshot](docs/evidence/screenshots/contact-desktop.png) |
| As a form user, I want confirmation after submitting. | The contact form redirects to `thankyou.html`. | [Thank you desktop screenshot](docs/evidence/screenshots/thankyou-desktop.png) |
| As a mobile or narrow-screen user, I want content to remain readable. | Layouts collapse to single columns and navigation stacks on narrow screens. | [Narrow screenshots](#screenshot-evidence) |

## Design Decisions

The design uses a calm blue palette, white cards, large headings and clear sections to support a friendly community gym identity. The structure is intentionally simple so users can scan the site without needing complex interactions.

Planning documents:

* [Brief and Goals](assets/brief-and-goals.pdf)
* [Sitemap / Information Architecture](assets/sitemap-ia.pdf)
* [Wireframes](assets/wireframes.pdf)
* [Resubmission checklist](RESUBMISSION_CHECKLIST.md)
* [Final evidence status](EVIDENCE_STATUS.md)
* [Final manual evidence steps](FINAL_MANUAL_STEPS.md)

## Website Features

* Consistent header navigation across all pages.
* Active navigation state using `aria-current="page"`.
* Home page hero, benefits, featured classes, trainer preview, membership call-to-action and testimonials.
* Classes page with class cards and timetable table.
* Trainers page with trainer profiles and coaching information.
* Membership page with plan cards and FAQs.
* Contact page with opening hours, contact details and form.
* Thank you page for form submission confirmation.
* Footer quick links and external social links.

## Accessibility

The resubmission feedback identified the previous interactive blue `#2f80ed` as approximately 3.87:1 against white text, below the expected 4.5:1 contrast ratio for normal text.

The interactive colour has been changed to `#005ea8`, which keeps the visual design similar while improving contrast:

| Colour use | Old ratio | New ratio | WCAG result |
| --- | ---: | ---: | --- |
| White text on `#2f80ed` | 3.87:1 | Not used for normal text | Failed normal text |
| White text on `#005ea8` | Not applicable | 6.63:1 | Passes AA normal text |
| White text on hover `#004b8d` | Not applicable | 8.78:1 | Passes AA normal text |

Keyboard focus has also been improved:

* Navigation links, logo, buttons, key text links and footer links use `:focus-visible`.
* Form inputs and textareas use a visible blue focus outline.
* Important interactive elements have a high-visibility focus treatment with a yellow outline and dark outer ring where needed.
* Manual keyboard tab-through verification is listed in [docs/testing.md](docs/testing.md) so it can be repeated before resubmission.

Other accessibility choices:

* Images include descriptive `alt` text.
* Tables use headings and, where appropriate, captions.
* Active page navigation uses `aria-current="page"`.
* Quote-only testimonial cards were changed from `article` to `div` to avoid misleading article semantics and HTML validator warnings.
* External links that open in a new tab include `rel="noopener noreferrer"`.

## Responsive Design

The stylesheet uses responsive media queries at 900px, 700px and 480px. On smaller screens, grids collapse to one column, navigation stacks vertically, and buttons become easier to tap. Headless Edge screenshots were generated locally for desktop and narrow viewport evidence.

## Screenshot Evidence

Screenshots were generated locally with Microsoft Edge headless on 10 May 2026. Desktop screenshots used a 1366px wide viewport. Narrow screenshots used a 500px wide viewport to evidence the responsive single-column layout.

| Page | Desktop evidence | Narrow evidence |
| --- | --- | --- |
| Home | [index-desktop.png](docs/evidence/screenshots/index-desktop.png) | [index-narrow.png](docs/evidence/screenshots/index-narrow.png) |
| Classes | [classes-desktop.png](docs/evidence/screenshots/classes-desktop.png) | [classes-narrow.png](docs/evidence/screenshots/classes-narrow.png) |
| Trainers | [trainers-desktop.png](docs/evidence/screenshots/trainers-desktop.png) | [trainers-narrow.png](docs/evidence/screenshots/trainers-narrow.png) |
| Membership | [membership-desktop.png](docs/evidence/screenshots/membership-desktop.png) | [membership-narrow.png](docs/evidence/screenshots/membership-narrow.png) |
| Contact | [contact-desktop.png](docs/evidence/screenshots/contact-desktop.png) | [contact-narrow.png](docs/evidence/screenshots/contact-narrow.png) |
| Thank You | [thankyou-desktop.png](docs/evidence/screenshots/thankyou-desktop.png) | [thankyou-narrow.png](docs/evidence/screenshots/thankyou-narrow.png) |

Additional local evidence generated on 25 May 2026:

* [Home 390px mobile screenshot](docs/evidence/screenshots/index-mobile-390.png)
* [Contact 390px mobile screenshot](docs/evidence/screenshots/contact-mobile-390.png)
* [Home 768px tablet screenshot](docs/evidence/screenshots/index-tablet-768.png)
* [Live GitHub Pages homepage screenshot](docs/evidence/screenshots/github-pages-live-home.png)
* [Live GitHub Pages page-load check](docs/evidence/screenshots/github-pages-live-check.txt)
* [Visible focus state screenshot](docs/evidence/manual-testing/focus-visible-nav-local.png)
* [Keyboard focus check](docs/evidence/manual-testing/keyboard-focus-check.txt)
* [Contact form redirect check](docs/evidence/manual-testing/contact-form-redirect.txt)
* [Local evidence checks](docs/evidence/manual-testing/local-evidence-checks.md)

## Validation Evidence

Fresh official validation evidence generated on 25 May 2026:

| Evidence | File |
| --- | --- |
| W3C HTML - index | [w3c-html-index.txt](docs/evidence/html-validation/w3c-html-index.txt) |
| W3C HTML - classes | [w3c-html-classes.txt](docs/evidence/html-validation/w3c-html-classes.txt) |
| W3C HTML - trainers | [w3c-html-trainers.txt](docs/evidence/html-validation/w3c-html-trainers.txt) |
| W3C HTML - membership | [w3c-html-membership.txt](docs/evidence/html-validation/w3c-html-membership.txt) |
| W3C HTML - contact | [w3c-html-contact.txt](docs/evidence/html-validation/w3c-html-contact.txt) |
| W3C HTML - thankyou | [w3c-html-thankyou.txt](docs/evidence/html-validation/w3c-html-thankyou.txt) |
| W3C CSS - style.css | [w3c-css-style-css.txt](docs/evidence/css-validation/w3c-css-style-css.txt) |

The final W3C HTML evidence reports 0 errors and 0 warnings for all six HTML pages. The final W3C CSS evidence reports 0 errors and 1 warning about matching solid button background and border colours, which is an intentional design choice for filled buttons.

Legacy validator exports are still stored in `assets/`, but the final resubmission evidence is under `docs/evidence/`.

Current final evidence tracking is documented in [EVIDENCE_STATUS.md](EVIDENCE_STATUS.md). [FINAL_MANUAL_STEPS.md](FINAL_MANUAL_STEPS.md) confirms there are no remaining manual evidence tasks before lecturer review.

## Lighthouse Evidence

Lighthouse was run against the live GitHub Pages homepage on 25 May 2026.

| Mode | Report | Performance | Accessibility | Best Practices | SEO |
| --- | --- | ---: | ---: | ---: | ---: |
| Desktop | [lighthouse-desktop-report.html](docs/evidence/lighthouse/lighthouse-desktop-report.html) | 87 | 100 | 96 | 100 |
| Mobile | [lighthouse-mobile-report.html](docs/evidence/lighthouse/lighthouse-mobile-report.html) | 85 | 100 | 96 | 100 |

## Testing

Detailed manual and resubmission testing evidence is documented in [docs/testing.md](docs/testing.md).

Testing stages:

* Code inspection and repository audit.
* Static searches for old contrast colours, focus selectors, missing `rel` attributes and external links.
* Local screenshot generation with Microsoft Edge headless.
* Manual testing matrix prepared for browser, keyboard, validator and Lighthouse checks.
* Final official W3C validation and Lighthouse checks to be completed manually because this environment does not include local W3C validator or Lighthouse tooling.

## Bugs and Fixes

| Issue | Fix | Status |
| --- | --- | --- |
| Button and active navigation blue did not meet 4.5:1 contrast with white text. | Replaced `#2f80ed` with `#005ea8` for normal interactive text states. | Fixed |
| Hover blue needed to remain readable. | Added darker hover blue `#004b8d`. | Fixed |
| Keyboard focus was not consistently visible. | Added `:focus-visible` styles for navigation, buttons, links and form controls. | Fixed |
| Quote-only testimonial cards used `article` without headings. | Changed those cards to `div` in `index.html` and `trainers.html`. | Fixed |
| Contact footer external links opened new tabs without `rel`. | Added `rel="noopener noreferrer"` to all `target="_blank"` social links. | Fixed |
| Evidence filenames used spaces, capitals, brackets and special characters. | Renamed evidence files to lower-case hyphenated filenames and updated README links. | Fixed |
| Official post-fix W3C and Lighthouse evidence cannot be produced locally here. | Added manual instructions and evidence locations. | To be completed manually |

## Deployment

The project is deployed using GitHub Pages from the `main` branch.

Deployment steps:

1. Push the final committed changes to GitHub.
2. In the repository settings, open Pages.
3. Confirm the source is the `main` branch.
4. Wait for GitHub Pages to rebuild.
5. Open the live URL and verify each page loads.

Live website:

https://abdulkadirkhoujja.github.io/codeinstitute-milestone-1-project/

## Development Lifecycle

The project followed a user-centred frontend workflow:

1. Planning: define the gym concept, target users, site goals, sitemap and wireframes.
2. Structure: build static HTML pages for the main user journeys.
3. Styling: apply a friendly visual style, responsive grids and reusable card/button patterns.
4. Content: add gym information, class details, trainer profiles, memberships and contact flow.
5. Testing: check navigation, responsive layouts, form redirect, validation and accessibility.
6. Resubmission refinement: address feedback on colour contrast, focus visibility, HTML semantics, external-link security, evidence filenames and documentation completeness.
7. Final submission preparation: refresh official validator evidence, run Lighthouse, verify GitHub Pages and submit with a clean commit history.

## Technologies Used

* HTML5
* CSS3
* Git and GitHub
* GitHub Pages
* Figma for planning and wireframes
* W3C validators for HTML and CSS validation
* Microsoft Edge headless for local screenshot evidence

## Project Structure

```text
index.html
classes.html
trainers.html
membership.html
contact.html
thankyou.html

css/
  style.css

images/
  site images

assets/
  planning and validation evidence

docs/
  evidence/
    screenshots/
    manual-testing/
  testing.md

RESUBMISSION_CHECKLIST.md
EVIDENCE_STATUS.md
FINAL_MANUAL_STEPS.md
```

## Future Improvements

* Online class booking.
* Membership sign-up flow.
* Individual trainer profile pages.
* Interactive timetable filtering.
* Embedded map for the contact page.

## Credits

Images were sourced from Pexels: https://www.pexels.com/

Validation tools:

* HTML Validator: https://validator.w3.org/
* CSS Validator: https://jigsaw.w3.org/css-validator/

## Author

Created by Abdul Khoujja for the Code Institute User-Centric Frontend Development Milestone Project.
