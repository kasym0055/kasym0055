# GitHub Profile Implementation Plan

> **For agentic workers:** Use superpowers:executing-plans. Implement in the current fresh checkout with one agent, per the user's instructions.

**Goal:** Publish an original, professional profile grounded in Kasymbek's projects and verifiable credentials.

**Architecture:** GitHub profile README with local SVG artwork and normal Markdown links. No app, build pipeline or external statistics service.

**Tech Stack:** Markdown, supported HTML, SVG.

**Spec:** [Profile design](../specs/2026-11-01-github-profile-design.md).

## Global constraints

- The user selected the dark/blue direction; continue authorized implementation without additional process approval rounds.
- Do not invent employment, seniority, language proficiency or certificates.
- Preserve team attribution and distinguish released software from work in progress.
- Repository language statistics do not establish individual proficiency.
- Keep project memory current and avoid unnecessary dependencies, tests or subagents for this documentation change.

## Review focus

- Narrow displays: stack project descriptions; do not require wide tables.
- Light theme: banner stays legible and the surrounding Markdown uses GitHub's own theme.
- Broken external images: use local artwork for the essential visual identity.
- Unsupported Markdown/HTML: validate using GitHub's rendered Markdown and inspect the result.
- Missing credential evidence: request the real Coursera URLs and leave certificates unclaimed until supplied.

## Task 1: Profile content and visual identity

Files: `README.md`, `assets/profile-header.svg`, `assets/section-*.svg`, `.gitignore`.

- [x] Create the original navy/blue banner and small theme-neutral technology tiles.
- [x] Replace the template README with the introduction, connections, three featured projects and concise technology groups.
- [x] Add the supplied HackAlem AI certificate and record the outstanding Coursera evidence in project status.
- [x] Keep preview output in ignored `.preview/`.

## Task 2: Verify and publish

- [x] Parse SVG as XML, run `git diff --check`, and inspect all local file references.
- [x] Check project sources and the existing FocusDuo release using read-only requests; preserve the supplied LinkedIn URL and record its access limitation.
- [x] Render through GitHub Markdown, inspect desktop dark/light and a narrow container; repair clipping or broken assets.
- [x] Update `docs/PROJECT.md` with validation results and remaining limitations.
- [ ] Publish the verified files as one profile update using native Git for binary artifacts, preserving any newer remote work.
- [ ] Verify the remote README and assets and synchronize the local checkout.

No application unit tests are needed: this change is documentation and artwork. Visual and link validation exercise the actual failure modes.
