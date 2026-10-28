# Joaquín Irazábal González — personal academic website

Static personal website of **Joaquín Irazábal González**, Assistant Research Professor in the Machine Learning in Civil Engineering group at **CIMNE**. The site focuses on machine learning and numerical simulation applied mainly to industrial engineering and dam safety.

The site follows the visual identity, navigation patterns and technical approach of the [MLCE group website](https://cimnemadrid.github.io/MLCE_Website/), but contains information about one person only.

**Live site:** <https://joaquinirazabal.github.io/JIG_Website/>

## File structure

- `index.html`: Home, short biography, research areas, selected projects and selected publications.
- `research.html`: Research lines and methods.
- `publications.html`: Journal articles and conference contributions.
- `projects.html`: Industrial engineering and dam safety projects, plus other projects.
- `about.html`: Career, education, award, contact details and academic profiles.
- `styles.css`: shared styles, responsive layouts and accessibility rules.
- `assets/images/`: portrait and CIMNE logo.
- `assets/favicon.svg`: site icon.
- `AGENTS.md`: repository guidance for future maintenance.

The website uses only HTML and CSS. No installation, build step or external dependencies are required.

## Content sources

Content was compiled in October 2026 from:

- FECYT CVN curriculum (`cvn_20261028104832974_1793180919542.pdf`), the primary source for positions, education, projects and publications.
- [ORCID 0000-0003-4966-4812](https://orcid.org/0000-0003-4966-4812), used to add publications not yet listed in the CV.
- [Google Scholar](https://scholar.google.es/citations?user=T08dTR4AAAAJ) and [Crossref](https://www.crossref.org/), used to confirm citation details, DOIs and citation metrics.
- [Scopus](https://www.scopus.com/authid/detail.uri?authorId=56823548200), used to verify the indexed document list and add the COMPDYN 2025 conference paper.
- [ResearchGate](https://www.researchgate.net/profile/Joaquin-Irazabal-Gonzalez) and [LinkedIn](https://www.linkedin.com/in/joaquinirazabalgonzalez/) for profile links.

Publication and project lists are curated snapshots, not live data. Update them manually when new outputs appear. Metrics on the home page (citations and h-index) come from Google Scholar and should be revised periodically.

## Local development

1. Clone the repository or open this folder.
2. Open `index.html` directly in a web browser, or serve the folder locally:

   ```bash
   python3 -m http.server 8000
   ```

   Then visit `http://localhost:8000/`.
3. Edit the HTML or CSS in your preferred text editor, save, and refresh the browser.

Keep all five HTML files and `styles.css` together at the repository root. Use relative page and asset paths so they work both locally and under the GitHub Pages repository path.

The navigation and footer are repeated in each HTML file. When changing either, update all five copies. Keep the same menu order and set `aria-current="page"` only on the current page's navigation link. All presentation rules belong in the shared stylesheet.

## Publish to GitHub Pages

The site is published with GitHub Pages from the `main` branch, `/(root)` folder:

- GitHub account: [joaquinirazabal](https://github.com/joaquinirazabal)
- Repository: <https://github.com/joaquinirazabal/JIG_Website>
- Published site: <https://joaquinirazabal.github.io/JIG_Website/>

To publish changes:

```bash
git add .
git commit -m "Describe the change"
git push origin main
```

GitHub Pages rebuilds automatically after each push to `main`. Check the deployment status in the repository's **Actions** tab. If the Pages configuration ever needs to be restored, go to **Settings → Pages**, choose **Deploy from a branch**, and select `main` and `/(root)`.

Local edits do not publish until committed and pushed. No custom workflow or build tooling is needed.

## Before publishing

- Check the desktop layout and a narrow mobile viewport.
- Follow each navigation link from every page and confirm the correct page is highlighted.
- Press Tab to reveal “Skip to content”, then Enter to move focus to the main content.
- Confirm that external profile and DOI links resolve.
- Review the publication and project lists for new entries.
