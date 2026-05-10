# Resubmission Checklist

This checklist maps the resit feedback to the repo changes needed before final submission.

## 1. UX, Accessibility and Responsivity

- [x] Replace the failed button, active navigation and key link blue `#2f80ed` where it is used with white or normal-sized text.
- [x] Use a visually similar darker blue that reaches at least 4.5:1 contrast against white.
- [x] Check hover and active states for readable contrast.
- [x] Add clear `:focus-visible` styles for navigation links, buttons, form controls, text links and footer links.
- [x] Document the old colour issue, new colour choice, contrast ratio evidence and keyboard focus checks in the README.

## 2. HTML and CSS Implementation

- [x] Fix HTML validator warnings in `index.html`, especially article elements without headings.
- [x] Fix HTML validator warnings in `trainers.html`, especially article elements without headings.
- [x] Add `rel="noopener noreferrer"` to every external link using `target="_blank"`.
- [x] Check all HTML files for external link security consistency.
- [x] Review CSS validator warnings and either fix them or document why they are harmless.
- [x] Re-run available validation checks after each implementation batch.

## 3. Maintainability and Documentation

- [x] Rename evidence files in `assets/` to lower-case, hyphenated filenames with no spaces, brackets, ampersands or special characters.
- [x] Update README links and any internal references after renaming evidence files.
- [x] Add finished website screenshots mapped to user stories where possible.
- [x] If screenshots cannot be generated locally, add a clear evidence table with exact filenames to capture manually.
- [x] Expand the README with project purpose, target users, user stories, design decisions, accessibility rationale, responsive design, testing stages, validation evidence, deployment evidence, bugs and fixes, future improvements and lifecycle narrative.

## 4. Version Control

- [x] Inspect repo structure before changes.
- [x] Check initial Git status before changes.
- [x] Make multiple small, meaningful commits.
- [x] Run `git status` before and after every commit.
- [x] Keep each commit working and feature-scoped.

## 5. Testing and Deployment Evidence

- [x] Add a detailed manual testing matrix with page, action, expected result, actual result, pass/fail and date.
- [x] Include tests for all pages, internal links, external links, responsive layouts, keyboard navigation, visible focus states, colour contrast, HTML validation, CSS validation and Lighthouse/performance evidence where possible.
- [x] Add a bugs and fixes table.
- [x] Add GitHub Pages deployment evidence.
- [x] Mark unavailable automated evidence as "to be completed manually" with clear instructions.
