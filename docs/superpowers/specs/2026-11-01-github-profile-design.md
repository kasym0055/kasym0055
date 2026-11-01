# GitHub profile design

Date: 2026-11-01. Status: implemented and published in the direction selected by the user. Detailed layout and copy were the agent's decisions within the authorized profile refresh.

## Intent

Make Kasymbek's profile memorable and credible within the first screen, then let visitors inspect his work and credentials. The examples inform hierarchy and atmosphere; artwork and copy will be original.

## Approaches considered

| Direction | Trade-off |
| --- | --- |
| Dark portfolio with blue accents — selected by user | Distinctive banner, concise project sections and readable content; easy to maintain |
| Monochrome editorial profile | Lowest visual complexity, but less expressive than the supplied examples |
| Animated atmosphere and statistics dashboard | More motion, but heavier assets and more dependence on external image services |

All use GitHub Markdown, a small amount of supported HTML and repository-owned SVG assets. No frontend framework, hosting bill or runtime is needed. SVG artwork is sharp and editable; standard text remains searchable and accessible.

## Layout and draft copy

1. **Banner.** Deep navy, electric-blue geometric paths, restrained grid, original abstract graphic. No copied anime imagery. Proposed text: `KASYMBEK TALASBEK` / `Software Developer · Mobile & Web` / `From a useful idea to a working product.`
2. **Introduction.** `I build mobile, desktop and web applications, and collaborate on products with KDvibers. My work spans Kotlin interfaces, web experiences and backend integration.` The broad title is an editorial proposal, not a claim of seniority or employment.
3. **Connect.** Direct links to the user's LinkedIn and KDvibers. Do not publish an account email simply because a connector exposes it.
4. **Selected work.** Three clearly separated projects with repository links, concise purpose, relevant stack and evidenced personal contribution:
   - **FocusDuo:** shared focus sessions with a synchronized timer, goals and session history. Highlight desktop work and Windows packaging; link the existing release.
   - **HackAtlas:** mobile discovery of hackathons. Highlight Kotlin Multiplatform client work and API/session integration. Label as in development, with no claim of a released iOS app.
   - **Forte Cash Audit:** a team project turning video uploads into reviewable reports. Highlight frontend, application backend and deployment. Attribute local AI analysis to the team rather than claim personal model development.
5. **Technologies.** Compact groups with restrained icons: Kotlin; Python; TypeScript / JavaScript; HTML / CSS; Compose, Android, FastAPI, React / Next.js, Git. Project-level Java/Spring Boot/PostgreSQL can appear beside the relevant projects; a team stack is not automatically a personal proficiency list. Add other languages when confirmed.
6. **Learning & credentials.** A short curated list of Coursera credentials with exact title, issuer and verification link; an expandable list for additional certificates if needed. No invented awards, completion dates or placeholder credentials. This section waits for the user's evidence.
7. **Closing contact.** A short invitation to discuss projects, linked to LinkedIn.

## Visual and technical constraints

- Banner roughly 1200 × 360, with enough empty space and large lettering to stay readable at profile width.
- Blue highlights should work with GitHub's dark and light themes. GitHub controls the surrounding page background; this design does not change the user's global theme.
- Keep essential copy as Markdown/HTML text rather than embedding all information in an image.
- Prefer stacked project sections to wide layouts that require horizontal scrolling on phones.
- Local SVG assets contain no scripts, external fonts or embedded remote content.
- Default to no external statistics cards: the native GitHub activity graph remains available, and project evidence deserves more space than counters. An optional stats addition can be considered later if requested.
- Preserve the distinction between individual contribution and organizational ownership.

## Acceptance and remaining input

The README should render cleanly on desktop and narrow screens, have working links and images, and accurately describe each project. Validate original assets and GitHub-compatible rendering; do not run unrelated application tests.

Remaining input: Coursera credential links or certificate files. The supplied HackAlem AI participation certificate confirms the display name and is included with its original PDF and an expandable image preview. Publication and live rendering have been verified; see `docs/PROJECT.md` for the evidence and handoff.
