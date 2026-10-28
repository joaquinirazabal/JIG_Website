# AGENTS.md — Personal website of Joaquín Irazábal González

## Project overview

This repository contains the public personal academic website of **Joaquín Irazábal González**, Assistant Research Professor in the **Machine Learning in Civil Engineering (MLCE)** group at **CIMNE** (International Centre for Numerical Methods in Engineering).

- **Website language:** English
- **Hosting:** GitHub Pages
- **Repository:** <https://github.com/joaquinirazabal/JIG_Website>
- **Live site:** <https://joaquinirazabal.github.io/JIG_Website/>
- **Primary audience:** Researchers, collaborators, project partners, prospective students and engineering professionals
- **Visual reference:** <https://cimnemadrid.github.io/MLCE_Website/>

The site deliberately reuses the visual identity and technical approach of the MLCE group website while containing information about one person only.

## Site structure

Keep the current five-page static structure and main navigation:

- Home (`index.html`): biography summary, research areas, selected projects and selected publications.
- Research (`research.html`): research lines and methods.
- Publications (`publications.html`): journal articles and conference contributions.
- Projects (`projects.html`): industrial engineering, dam safety and other projects.
- About (`about.html`): career, education, award, contact and profiles.

Do not create additional pages, menu items or sections without an explicit request. Preserve the single shared `styles.css`. Use the same navigation and footer on every page, with relative page links and `aria-current="page"` on the current navigation item. Keep duplicated navigation and footer markup synchronized manually; no build step is required.

## Technical constraints

- Prefer **semantic HTML and plain CSS**.
- Use JavaScript only when it provides a clear functional benefit.
- **Do not introduce** React, Vue, Bootstrap, Tailwind, package managers, build pipelines or external libraries without explicit approval.
- Keep `index.html` at the repository root so GitHub Pages can serve it.
- Use relative links and asset paths compatible with deployment under `https://joaquinirazabal.github.io/JIG_Website/`.
- Avoid unnecessary dependencies, scripts, animations and large assets.

## Content rules

- Write website copy in clear **English**, with concise and technically accurate wording.
- Do not invent achievements, positions, publications, projects, dates, funding figures or institutional endorsements.
- Use the FECYT CVN curriculum as the primary source for career, education, projects and publications. Cross-check newer outputs with ORCID, Google Scholar, Crossref or Scopus before adding them.
- Do not publish sensitive personal data from the CV (DNI, home address, phone numbers, date of birth).
- Publication lists are curated snapshots. When adding an entry, include authors, venue, volume/issue, pages or article number, year and DOI when available.
- Metrics shown on the home page come from Google Scholar and must be labelled and updated deliberately.
- Treat unverified details as drafts requiring confirmation.

## Design and accessibility

- Style: **simple, clean, modern, academic and professional**.
- Preserve readability, generous whitespace and a responsive layout for desktop, tablet and mobile.
- Reuse CSS variables and existing classes rather than adding one-off styles.
- Use logical heading hierarchy, semantic landmarks and descriptive link text.
- Provide meaningful alt text for informative images and empty alt text for decorative ones.
- Ensure keyboard accessibility, visible focus states and readable contrast.
- Respect `prefers-reduced-motion` where motion is used.
- Check links between all five pages, current-page highlighting, and the skip-to-content anchor beneath the sticky header on small screens.

## Workflow for agents

1. Inspect the relevant files before making changes.
2. Make the **smallest focused change** that satisfies the request.
3. Preserve existing approved content, navigation, visual design and working behavior unless a change is explicitly requested.
4. If content is missing or uncertain, flag the gap instead of making up facts.
5. After changes, check internal links, responsive behavior and relevant accessibility concerns as far as available tools allow.
6. Summarize which files changed, what was changed, and what the user should verify in the browser.
7. **Never commit, push or deploy automatically.** The user handles Git and publication personally. Do not run `git add`, `git commit`, `git push` or a GitHub Pages deployment unless the user explicitly requests that specific action in the current message.
8. Leave the working tree with the requested changes so the user can review and commit them.

## Git and publication

The user controls the repository and the live site. Agents must stop after editing, validating and summarizing the changes.

- Do not create commits.
- Do not push to `origin`.
- Do not trigger or modify GitHub Pages deployments.
- Do not run commands that stage changes automatically (for example, `git add .`).
- If a commit or push seems necessary, ask the user first and wait for explicit confirmation.

The live site is <https://joaquinirazabal.github.io/JIG_Website/> and publishes from `main`. Changes remain local until the user commits and pushes them.

## Reference URLs

- Group website: <https://cimnemadrid.github.io/MLCE_Website/>
- CIMNE: <https://cimne.com/>
- ORCID: <https://orcid.org/0000-0003-4966-4812>
- Google Scholar: <https://scholar.google.es/citations?user=T08dTR4AAAAJ>
- Scopus: <https://www.scopus.com/authid/detail.uri?authorId=56823548200>
- ResearchGate: <https://www.researchgate.net/profile/Joaquin-Irazabal-Gonzalez>
