# beta-industries

Three linked HTML pages (home, about, contact) for navigation + form-trigger tests. Default persona: **Beta Industries** (also serves multi-container CL-MUL tests).

**Live URL:** `https://cpaynejz.github.io/beta-industries/`

## Test plan scenarios served

- TC-3.1.4 sub-paths
- TC-3.1.8 site URL with subpath (run Discovery against `.../beta-industries/about.html`)
- TC-1.1.* event-tag scenarios using form-submit / linkClick triggers (the contact page has both)
- TC-3.2.11 / TC-3.2.12 multi-container — paste both BETA-MAIN and BETA-SECONDARY snippets in the same HTML files
- Multi-page-view event tracking validation

## How to configure

Paste the same GTM snippet into all three HTML files (`index.html`, `about.html`, `contact.html`) at the marked head + body locations. Commit and push.

## Notes

- The form on `contact.html` does not POST — it intentionally just toggles a confirmation message. This lets a Form Submission GTM trigger fire without page navigation.
- `mailto:` and `tel:` links on the contact page exercise the linkClick trigger built-in.
