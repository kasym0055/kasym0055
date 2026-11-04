# GitHub profile refresh

Updated: 2026-11-01. Repository: https://github.com/kasym0055/kasym0055

## Goal and scope

Create a distinctive, professional GitHub profile inspired by the user's two screenshots. Make actual projects, personal contributions, technologies, Coursera credentials and LinkedIn easy to find. Work in the existing profile repository; no separate website or paid hosting is needed.

## Confirmed decisions

- Current direction (2026-11-04): use English, GitHub's native typography and real application screenshots. The FocusDuo demo is visible in the project story and the HackAtlas calendar opens on demand.
- English was proposed as the profile language alongside that selection.
- LinkedIn supplied by the user: https://www.linkedin.com/in/kasymbek-talasbek-7ba212378/
- Include projects from the user's KDvibers organization.
- Do not copy the examples, invent skills or credentials, or attribute a teammate's work to the user.
- Work with one agent. Keep research and verification proportional to a README change.

## Evidence collected

Read through the GitHub connector and public GitHub API on 2026-11-01:

| Source | Verified content | Personal attribution / caveat |
| --- | --- | --- |
| [Profile README](https://github.com/kasym0055/kasym0055/blob/main/README.md) | Default greeting only; cloned into this workspace | Original README blob: `2546fc0275041791579e1bcd3f5d0643697ba462` |
| [FocusDuo](https://github.com/KDvibers/FocusDuo) | Shared focus sessions; Kotlin/Compose Desktop, Java/Spring Boot, PostgreSQL; Windows 0.1.0 release | `kasym0055` authored desktop MSI packaging commit `95e36d7e2c066152e538a72d0bb8f1501a556ece`; do not claim sole backend authorship |
| [HackAtlas](https://github.com/KDvibers/HackAtlas) | Kotlin Multiplatform / Compose mobile hackathon catalogue and Java backend | `kasym0055` mobile commits include secure session client, registration links and native share; Android checked in project docs, iOS verification still pending |
| [Forte Cash Audit](https://github.com/KDvibers/forte-cash-audit#team) | Team case project: video upload, local analysis and evidence reports | README explicitly attributes frontend, results UI, application backend and Funnel deployment to Kasymbek; analyzer belongs to Daniyar |
| [Playlist_Maker2](https://github.com/kasym0055/Playlist_Maker2) | Kotlin Android project; default branch `dev` | No README; Gradle manifest checked. Do not infer full music features from its name |
| [locus-hackathon](https://github.com/kasym0055/locus-hackathon) | TypeScript, Next.js, React, Redis dependencies | No README; default branch `feat/m1-vertical-slice`. Avoid featuring without a clear product summary |
| [Wedding invitation](https://github.com/kasym0055/azamat-ayaulym-wedding) | HTML/CSS/JavaScript | Optional secondary work; no need to feature private event details |

Repository language statistics are evidence of technology use in projects, not proof of individual proficiency. The older Legend repository includes PHP/Hack/CSS; dependency attribution has not been checked, so these statistics must not become automatic skill claims.

## Open facts

- Coursera: 52 distinct certificate-issued confirmations found through the connected Gmail account. The user supplied a public share URL for one certificate; its canonical verification page, learner, course, provider and date have been checked. Public links for the other 51 courses remain unavailable.
- LinkedIn connector search found no matching profile, and public fetch returned HTTP 999. The user's exact URL is available, but profile content and certifications were not retrieved.
- Display name `Kasymbek Talasbek` is confirmed by the supplied HackAlem AI participation certificate. The broad developer title avoids inventing seniority or employment.
- Java was explicitly confirmed by the user's request to add it to the toolkit; additional languages still require evidence or user confirmation.

## Milestones and handoff

1. Research and choose direction — complete.
2. Record selected direction — complete; see [design](superpowers/specs/2026-11-01-github-profile-design.md). Detailed layout decisions were made within the user's authorized request.
3. Implement README, local artwork and credential section — complete for available evidence, including the 52-course Coursera catalogue and one public credential.
4. Check links, image rendering, mobile readability, light/dark compatibility and factual attribution — complete locally.
5. Publish the profile update and verify the live result — complete for all supplied evidence.

Next step: attach public verification links for the remaining 51 Coursera courses when supplied. Do not replace them with private dashboard or email tracking URLs.

### Profile simplification · 2026-11-04

Follow-up: the user asked for a little more creativity within the natural style. The profile now shows a demo room from FocusDuo, an expandable HackAtlas calendar, and Kasymbek's commit for the Windows installer. The two images come from the project repositories. Exact source revisions are recorded in [asset attribution](../assets/ATTRIBUTION.md).

The user asked to remove the illustrated studio banner and make the profile sound more natural. The main README now starts with the developer's name, a short introduction and a link to the Windows release. The three KDvibers projects are described in first person, with specific contributions and teammate credit. The toolkit is plain text and still includes Java. The credentials section links to the HackAlem PDF, the complete Coursera list and the verified Wiley credential. LinkedIn remains a plain link. Certificate details and the original Wiley preview live in the catalogue. The studio banner file is removed; the other artwork is no longer displayed in the profile.

## HackAlem AI certificate

The user supplied a one-page image-based PDF and explicitly requested its inclusion. Visual inspection confirms: Kasymbek Talasbek; Certificate of Participation; HackAlem AI; Astana, Kazakhstan; November 1, 2026. The Guinness World Records statement belongs to the event and is attributed to the certificate, not presented as an individual prize or independent verification.

- Original preserved at `certificates/hackalem-ai-2026-kasymbek-talasbek.pdf`; SHA-256 equality with the supplied file checked.
- Preview at `assets/certificates/hackalem-ai-2026.png`, rendered using Poppler.
- No external verification link was extracted from the PDF; no independent organizer verification was performed.

## Validation record

- All three original SVG files parsed as XML and contain no scripts or foreignObject content.
- All six unique local README file references resolve; `git diff --check` passed.
- GitHub's Markdown API rendered the README successfully, including supported HTML and the certificate disclosure.
- Browser inspection of that rendered HTML passed in dark and light themes; all four images loaded.
- At 390 px container width, content width equals client width (388 px): no horizontal overflow. Certificate disclosure opens and displays its preview.
- Existing FocusDuo v0.1.0 release and MSI asset confirmed through the GitHub connector.
- LinkedIn destination is the exact user-supplied URL. Its content could not be independently read.
- Local preview uses approximate GitHub CSS. After publishing commit `d7f3c98`, the actual GitHub profile was inspected in the browser: all four images loaded, the credentials navigation reached its target, and the disclosure displayed the certificate correctly.
- The original binary PDF and PNG preview are present in the published repository. The final cleanup removes a redundant custom anchor where GitHub already generates a heading anchor.

## Workflow decisions

Use the existing fresh checkout and `feat/profile-refresh` branch. No application unit tests, dependencies, automation workflows or extra agents are needed for Markdown and artwork. Native Git publication is appropriate for this local change because it includes the original binary PDF and image preview; the GitHub connector was used for source and release verification.

## Creative revision requested by the user

The user found the first design boring and asked for more creativity. The revision keeps the dark/blue direction and factual content, adds an original ImageGen studio illustration, conceptual project covers, subtle SVG motion, recognizable language icons, contact buttons and an achievement badge. Visible descriptions are shorter; technical details use labeled disclosures.

See [creative notes and final ImageGen prompt](superpowers/specs/2026-11-01-creative-refresh.md) and [asset attribution](../assets/ATTRIBUTION.md). The hero is stored locally in `assets/profile-hero-v2.png`; the original generated file and old SVG header remain preserved.

Checks: all 10 SVGs parse, 12 linked local files exist, GitHub Markdown rendering succeeds, all 11 images load, desktop dark/light and a 390 px container have been inspected. No narrow-container overflow (388 px client/content width). Project and certificate disclosures open correctly. The FocusDuo SVG reports a 32-second CSS animation, with different transforms observed in two reads; reduced-motion CSS is present but the OS preference was not changed for testing. Corrected cover spacing and the achievement badge's polygon geometry during visual QA. Published in commit `2e3278e`; the live GitHub profile shows the new hero and project cards, all 11 profile images loaded, and the FocusDuo disclosure exposes the expected content.

## Java and Coursera follow-up

The user requested Java in the toolkit and asked about Coursera. Seven individually wrapping local SVG tiles now include Java, using the Devicon symbol with its MIT attribution. The six existing language paths are preserved.

The connected Gmail account contains certificate-issued confirmations for 52 distinct courses. Only course titles and providers were extracted into the public catalogue; message content, addresses, message IDs and tracking URLs are not published. The email buttons redirect to the generic private accomplishments area. A Drive search returned no certificate files.

The user then supplied `https://coursera.org/share/b976463a402c2690168959fda1879397`. It resolves to [credential RVE17IID343O](https://www.coursera.org/account/accomplishments/verify/RVE17IID343O), confirming **Kasymbek Talasbek**, **Driving Growth, Leadership, and Continuous Improvement**, **John Wiley & Sons**, **October 31, 2026**. The original public JPEG is stored locally; README includes the verification link and a collapsible preview. The full catalogue accurately distinguishes course certificates from the Cisco CCNA exam credential and explains the unavailable verification links for other courses.

Validation: all eight new SVGs parse and have no executable content; seven language tiles and the Coursera card were rasterized with Sharp and visually inspected. The public certificate image was inspected. Both README files rendered successfully through GitHub's Markdown API; all local references resolve; the catalogue has exactly 52 course rows; `git diff --check` passed. Full browser/mobile reinspection is unavailable because local browser use is disabled in Work settings.
