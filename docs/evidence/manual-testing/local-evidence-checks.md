# Local Evidence Checks

Audit date: 25 May 2026

These checks were completed locally by Codex. They are supporting evidence only and do not replace fresh official W3C, Lighthouse or live GitHub Pages evidence.

| Check | Result | Evidence |
| --- | --- | --- |
| `index.html` article-heading source check | `articles=12`, `article-without-heading=0` | Current `index.html` source |
| `trainers.html` article-heading source check | `articles=9`, `article-without-heading=0` | Current `trainers.html` source |
| All HTML files article-heading source check | No `article` elements without headings found | Local Node source scan |
| CSS brace and old-colour check | Final brace depth `0`; `:focus-visible` present; old `#2f80ed` absent | Current `css/style.css` |
| External new-tab link security | `target-blank-missing-rel=0` | Local Node source scan |
| Local HTML links/assets | `local-html-link-check failures=0` | Local Node source scan |
| Contact form action | Form uses `action="thankyou.html"` and `method="get"` | `contact.html` |
| 390px home screenshot | Captured at `390x900` | `docs/evidence/screenshots/index-mobile-390.png` |
| 390px contact screenshot | Captured at `390x900` | `docs/evidence/screenshots/contact-mobile-390.png` |
| Tablet home screenshot | Captured at `768x900` | `docs/evidence/screenshots/index-tablet-768.png` |
| Focus-visible screenshot | Captured with the Classes navigation link focused | `docs/evidence/manual-testing/focus-visible-nav-local.png` |
