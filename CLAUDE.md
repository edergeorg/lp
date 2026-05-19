# CLAUDE.md — Lisa Posch Physiotherapie

## Project

One-page website for physiotherapist Lisa Posch (Vienna).
**Goal:** High organic search ranking + clear CTA to book appointments via Appointmed.
**Audience:** German-speaking patients in Vienna looking for physiotherapy.

## Authorship

Always present in the codebase:
- **Author:** Georg Eder
- **Contact:** hallo@ederge.org

Include in the HTML comment header of `index.html`, in `<meta name="author">`, and in JSON-LD schema where appropriate.

## Stack

- **Language:** Plain HTML5 / CSS3 / vanilla JS — single `index.html`, no build tools
- **Fonts:** Google Fonts (Cormorant Garamond + DM Sans) via preconnect — no cost
- **Booking:** Appointmed — external link/embed only, no API, no cost risk
- **Hosting:** GitHub (Pages or similar)
- **No frameworks, no npm, no bundler** — keep it that way unless explicitly approved

## Code Conventions

- **Indentation:** 2 spaces
- **CSS classes:** kebab-case, BEM naming where structure benefits from it
- **HTML:** semantic elements — `<section>`, `<nav>`, `<main>`, `<article>`, `<footer>`
- **CSS variables:** all colors/spacing defined in `:root`, no magic numbers scattered in rules
- **No inline styles** — exception: JS-driven dynamic values only
- **Comments:** English only, only where the WHY is non-obvious
- **Commits:** Conventional Commits in English — `feat:`, `fix:`, `docs:`, `refactor:`, `style:`, `perf:`
- **No new external dependencies** without prior approval

## Workflow

1. **Plan Mode first** for any non-trivial change — propose approach, wait for approval
2. **Implement**
3. **Self-review checklist** (see below)
4. **Report** what changed and what needs manual verification

## Checklist After Every Change

- [ ] HTML is valid — no broken nesting, correct heading hierarchy (h1 → h2 → h3)
- [ ] Responsive at 375px, 768px, 1280px
- [ ] Lighthouse targets: Performance ≥ 90, SEO ≥ 95, Accessibility ≥ 90
- [ ] CTA (Appointmed link) visible above the fold on mobile
- [ ] Page weight: no new assets without compression/optimization
- [ ] Author meta and JSON-LD schema intact

## SEO Rules

- `<title>`: max 60 characters; `<meta name="description">`: max 155 characters
- JSON-LD `LocalBusiness` schema must stay intact and accurate
- Every image needs a descriptive `alt` attribute
- Heading hierarchy must be logical — never skip levels for styling reasons
- Internal anchor links must use meaningful `id` attributes

## External Services & Cost Awareness

| Service | Usage | Cost risk |
|---|---|---|
| Appointmed | Booking CTA link | None |
| Google Fonts | Preconnect load | None |

**Rule:** Before integrating any new external service or API, estimate the cost and name it explicitly before proceeding.

## Communication

- **Language:** Answer in German; code, comments, and commits in English
- **Style:** Direct and concise — no lengthy explanations unless asked
- **Address:** Use "du"
- **"mach mal"** = execute immediately, no clarifying questions
- **Sparring partner:** Challenge assumptions, find blind spots, don't just agree
- **Risks first:** If a decision has downsides, name them before saying yes
- **No flattery:** Skip "Großartige Idee!", "Absolut richtig!", and similar filler

## Don'ts

*(None defined yet — add here as the project evolves)*
