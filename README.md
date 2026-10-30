# Juanjo García Mesa — personal website

A responsive, static personal website for GitHub Pages. Plain HTML and CSS; no build step, dependencies, or JavaScript required.

## Preview locally

From this folder:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open http://localhost:8000. Stop the server with Ctrl+C.

## Edit content

- `index.html`: biography, projects, experience, publications, and community roles. The section IDs match the navigation links.
- `styles.css`: layout, responsive styles, and color variables at the top.
- `assets/juanjo-garcia-mesa.png`: headshot from the ASU directory, used with the site owner's authorization.
- `assets/favicon.svg`: initials favicon.

The site intentionally excludes an email address and downloadable CV. No analytics, external font requests, or third-party scripts are included. The image is served locally.

## Publish for free on GitHub Pages

1. Create a **public**, empty repository named **jgarciamesa.github.io** under the **jgarciamesa** account. Leave the README, license, and .gitignore options unchecked because the local site is already prepared.
2. Push this folder to that repository. From this folder, if it is not already a Git repository:

   ```sh
   git init -b main
   git add .
   git commit -m "Add personal research software engineering website"
   git remote add origin https://github.com/jgarciamesa/jgarciamesa.github.io.git
   git push -u origin main
   ```

3. In the repository, go to **Settings → Pages**.
4. Set **Source** to **Deploy from a branch**, select **main** and **/ (root)**, then save.
5. Visit **https://jgarciamesa.github.io/** once deployment completes. GitHub notes that publication can take up to 10 minutes.

`.nojekyll` tells GitHub Pages to serve the static files directly. No paid hosting or custom domain is needed.

Official instructions: https://docs.github.com/en/pages/quickstart

## Content provenance and maintenance

Content is based on the owner's CV and clarifications, with public project and publication links. No CV PDF is included in the repository.

- Role: Research Software Engineer, Computational Research Accelerator, ASU; responsibilities supplied by the owner.
- AlphaFold 3: adapted an existing pipeline for ASU HPC architecture, approximately 20,000 samples, viral protein against human proteome sequences, ipTM scoring for downstream candidate selection. No unconfirmed speedup, technology stack, or scientific result is claimed.
- RMACC Vice Chair: 2025–2026; term ends in December 2026. Update this entry after the term ends.
- CaRCC: content and review contribution through the working group, confirmed by the owner. https://carcc.github.io/CaRCC-AI-Facilitation-Handbook/authors/
- RAG: https://github.com/jgarciamesa/US-RSE24-RAG
- COATi: https://github.com/CartwrightLab/coati
- ASU profile and portrait: https://search.asu.edu/profile/2741263

The CV names the doctorate Biological Design; the site uses that degree title. The ASU profile describes the area as Bioinformatics.

The palette is inspired by ASU, with no university logos. This is a personal website.
