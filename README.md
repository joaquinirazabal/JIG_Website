# Joaquín Irazábal González — personal academic website

Static personal website of **Joaquín Irazábal González**, Assistant Research Professor in the Machine Learning in Civil Engineering group at **CIMNE**.

The site follows the visual identity, navigation patterns and technical approach of the [MLCE group website](https://cimnemadrid.github.io/MLCE_Website/), but contains information about one person only.

## File structure

- `index.html`: Home, short biography, research areas and selected publications.
- `research.html`: Research lines and methods.
- `publications.html`: Journal articles, conference contributions and preprints.
- `projects.html`: Selected projects and a list of further projects.
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
- [Scopus](https://www.scopus.com/authid/detail.uri?authorId=56823548200), [ResearchGate](https://www.researchgate.net/profile/Joaquin-Irazabal-Gonzalez) and [LinkedIn](https://www.linkedin.com/in/joaquinirazabalgonzalez/) for profile links.

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

GitHub account: [Joaquin-irazabal](https://github.com/Joaquin-irazabal). Repository: `JIG_Website`.

1. Create a new **public** repository named `JIG_Website` at <https://github.com/new>. Do not initialise it with a README, license or `.gitignore`.
2. Connect this local repository and push:

   ```bash
   git remote add origin https://github.com/Joaquin-irazabal/JIG_Website.git
   git push -u origin main
   ```

3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select `main` and `/(root)`, then **Save**.
6. Check the deployment status in the **Actions** tab and the published URL in **Settings → Pages**.

Expected website address: [joaquin-irazabal.github.io/JIG_Website](https://joaquin-irazabal.github.io/JIG_Website/).

Local edits do not publish until committed and pushed to `main`. No custom workflow or build tooling is needed.

## Before publishing

- Check the desktop layout and a narrow mobile viewport.
- Follow each navigation link from every page and confirm the correct page is highlighted.
- Press Tab to reveal “Skip to content”, then Enter to move focus to the main content.
- Confirm that external profile and DOI links resolve.
- Review the publication and project lists for new entries.
