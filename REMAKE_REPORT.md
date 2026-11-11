# Remake report: clinia.com → ProjectSuccess website

Date: 11.11.2026
Reference: https://clinia.com/ (style and structure only)
Tracking board: https://github.com/users/riekeschmidttreetops-tech/projects/1 ("Remake", no cards yet)
Output: `index.html` in this folder (one file, no build step)

## What was taken from Clinia, and what was not

Taken (design language only):
- Cream background, near-black text, tan accent on one phrase per headline
- Light serif headlines, small uppercase monospace labels and buttons
- Muted body text, one dark highlight card per row, light/dark toggle
- Section order: hero → 3 features → example "story" cards → 3-step tabs → 2 product cards → proof band → security grid → CTA cards → footer with large wordmark

Not taken: Clinia's name, logo, text, images, fonts (theirs are commercial), testimonials or certifications.
All copy is ProjectSuccess's own, written from the project docs (pilot format, two approvals, ICP rule,
UK GDPR / PECR / TPS / CTPS, 30-day deletion). Fonts are Fraunces, Inter and JetBrains Mono (SIL OFL,
fine for commercial use).

## Sections built

| # | Section | ProjectSuccess content |
|---|---------|------------------------|
| 1 | Hero | "Your CRM knows who to call next" + animated example call list |
| 2 | Features | Your rules from your history · two approvals · messy data is fine |
| 3 | Story cards | 4 made-up companies (win-back, former pilot, duplicates, sales dropped), labelled as made up |
| 4 | How it works | 3 tabs: read and check CRM · work out who to call · approve and track |
| 5 | Product | Head of Sales dashboard (light card) · BDM Monday list (dark card) |
| 6 | Free pilot | 2 + 2 weeks, results call, deletion within 30 days |
| 7 | Data & trust | UK GDPR · TPS/CTPS · 2 approvals · clean exit (no certifications claimed) |
| 8 | CTA | Book a 15-minute call · how the weekly run works |
| 9 | Footer | Links, © year, large wordmark |

## Checks done (11.11.2026, served at http://localhost:8770)

- [x] Page loads, no console errors, fonts load
- [x] Desktop 1024 px: every section checked by screenshot
- [x] Step tabs switch panels
- [x] Anchor links land below the sticky header
- [x] Phone 375 px: no sideways scrolling, menu opens and closes, cards stack
- [x] Dark mode (system setting and toggle), choice remembered per browser
- [x] Reduced-motion users get no animations

## Open before going live (founder)

1. Contact link: the "Book" button uses the placeholder `mailto:hello@example.com`. Replace it with the real address or a booking link.
2. Company name in the footer once the UK Ltd exists.
3. Google Fonts send each visitor's IP address to Google. For UK GDPR, self-host the three fonts before launch (or add them to the privacy notice).
4. A privacy notice / cookie page (the site sets no cookies; it only uses local storage for the theme).
5. Hosting and a domain. Nothing is published yet.
6. The trust statements must stay true (for example the 30-day deletion).

To preview: start "website" in the Claude preview pane (`.claude/launch.json` in ProjectSuccess), or run
`python -m http.server 8770 --directory .` in this folder.

Status: built by hand, NOT by the remake tool. The tool (github.com/riekeschmidttreetops-tech/remake) could not
be reached on 11.11.2026 (404; the account showed no public repositories). Later the same day a public repo
github.com/riekeschmidttreetops-tech/Remake appeared, but it only holds a README with the word "Remake":
no code, no instructions, no report. There is no remake tool to run.
