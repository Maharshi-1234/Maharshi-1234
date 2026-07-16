<div align="center">

# Ramana Maharshi Mellacheruvu — Portfolio

**AI Engineer | Bioinformatics**

[![Live Site](https://img.shields.io/badge/Live-Portfolio-059669?style=for-the-badge)](https://maharshi-1234.github.io/portfolio/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Deploy](https://img.shields.io/github/actions/workflow/status/Maharshi-1234/portfolio/deploy.yml?branch=main&style=for-the-badge&label=Deploy)](../../actions)

[LinkedIn](https://linkedin.com/in/m-ramana-maharshi) • [GitHub](https://github.com/Maharshi-1234) • [Hugging Face](https://huggingface.co/RamanaMaharshi)

</div>

---

## Overview

A single-page, animated portfolio site built to showcase work at the intersection of **AI/ML and Bioinformatics** — computational drug discovery, RNA-Seq/transcriptomics analysis, immunoinformatics, and healthcare data systems. Includes experience, certifications, and academic research projects, with a clean, minimal design and subtle scroll-based motion.

## Tech Stack

- **HTML5** — single-file, no build step required
- **Tailwind CSS** (via CDN) — utility-first styling
- **Lucide Icons** — lightweight icon set
- **Google Fonts** — Inter (UI) + JetBrains Mono (technical accents)
- **Vanilla JS** — scroll-reveal animations, mobile nav, tap-to-reveal certificate cards

No frameworks, no bundlers, no dependencies to install — open `index.html` and it runs.

## Project Structure

```
.
├── index.html                  # The entire site (single-page)
├── assets/
│   └── certs/                  # Certificate images (see assets/certs/README.md)
│       ├── ai-in-healthcare.jpg
│       ├── genetic-engineering-nptel.jpg
│       ├── complex-biological-systems-nptel.jpg
│       ├── linguaskill-business-cambridge.jpg
│       └── pet-cambridge.jpg
├── .github/
│   └── workflows/
│       └── deploy.yml          # Auto-deploys to GitHub Pages on every push to main
├── LICENSE
└── README.md
```

## Sections

| Section | Contents |
|---|---|
| **Hero** | Name, title, degree summary, rotating skill marquee |
| **Experience** | Bioinformatics Programmer (Biops Solutions), AI in Healthcare Internship (Ethical Edufabrica, IIT-KGP affiliated), Drug Discovery workshop (Decode Life) |
| **Certifications** | AI in Healthcare, Genetic Engineering (NPTEL), Complex Biological Systems (NPTEL), Linguaskill Business (Cambridge), PET (Cambridge) — hover/tap to reveal certificate image |
| **Academic Projects** | Phytocompound-based HMPV screening, in-silico SARS-CoV-2 vaccine design, personalized drug recommendation system, epitope mapping, healthcare data-standards web app |
| **Education** | B.Tech Bioinformatics (VFSTR), Intermediate (BIPC), SSC |
| **Contact** | Email, phone, LinkedIn, GitHub, Hugging Face |

## Certification Images — Placeholder Status

Certificate cards currently render a **dashed placeholder** on hover/tap. This is intentional — actual certificate images will be added directly to this repository. Each card is already wired to a specific expected filename under `assets/certs/`; once a matching image is committed, it appears automatically with **no HTML changes required**. Full naming convention: [`assets/certs/README.md`](assets/certs/README.md).

## Running Locally

No build step — just open the file:

```bash
git clone https://github.com/Maharshi-1234/portfolio.git
cd portfolio
open index.html        # macOS
# or: start index.html   (Windows)
# or: xdg-open index.html (Linux)
```

Or serve it (recommended, avoids any `file://` quirks):

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deployment (GitHub Pages)

This repo ships with a GitHub Actions workflow (`.github/workflows/deploy.yml`) that automatically builds and deploys to GitHub Pages on every push to `main`.

**One-time setup after pushing this repo:**
1. Go to **Settings → Pages**
2. Under **Build and deployment → Source**, select **GitHub Actions**
3. Push to `main` — the workflow deploys automatically
4. Your site goes live at `https://<your-username>.github.io/<repo-name>/`

## Updating Content

Since this is a single static file, all content lives in `index.html`:
- Experience entries: `<section id="experience">`
- Certifications: `<section id="certifications">`
- Projects: `<section id="projects">`
- Contact details: `<footer id="contact">`

## Contact

- **Email:** mellacheruvuramanamaharshi@gmail.com
- **Phone:** +91 8330945548
- **Location:** Guntur, Andhra Pradesh, India

## License

Licensed under the [MIT License](LICENSE) — feel free to fork the structure for your own portfolio, but please swap out personal content and credentials.
