# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a static personal portfolio website for Hsuan-Ming Chi, built on the "Massively" template by HTML5 UP. It is deployed as a GitHub Pages site (`https://alanchi0720.github.io/Hsuan-MingChi.github.io/`). There is no build system, package manager, or server-side code.

## Serving Locally

Open any `.html` file directly in a browser, or use any static file server. For example:

```bash
python -m http.server 8080
```

## Site Structure

| File | Purpose |
|---|---|
| `index.html` | Home page — project gallery with featured and grid post layout |
| `generic.html` | Resume page |
| `elements.html` | "Outside of Work" personal page |

## Styling

CSS lives in `assets/css/main.css` and `assets/css/noscript.css`. The source SCSS is in `assets/sass/` (structured as `base/`, `components/`, `layout/`, `libs/`). The compiled CSS is already committed — if you edit SCSS, you need to recompile manually with a Sass tool (e.g., `sass assets/sass/main.scss assets/css/main.css`). There is no watch script configured.

## JavaScript

All JS in `assets/js/` is third-party (jQuery, Scrollex, Scrolly, browser.min, breakpoints.min, util). The only custom logic is in `assets/js/main.js`.

## Adding a New Project Card

Projects are `<article>` elements inside `<section class="posts">` in `index.html`. Featured projects use `<article class="post featured">` above that section. Each card follows this pattern:

```html
<article>
    <header>
        <h2><a href="GITHUB_URL">Project Title<br /></a></h2>
    </header>
    <a href="#" class="image fit"><img src="images/your-image.jpg" alt="" /></a>
    <p>Short description.</p>
    <ul class="actions special">
        <li><a href="GITHUB_URL" class="button">Full Story</a></li>
    </ul>
</article>
```

## Images

Project images are stored directly in `images/`. Use descriptive filenames. Always use forward slashes in image paths (e.g., `images/file.jpg`) — backslashes break on GitHub Pages.

## Skills

The `frontend-design` skill is installed for this project. Use `/frontend-design` when building or redesigning UI components, pages, or sections to get production-grade, distinctive frontend output.

---

## Owner CV Reference

Use the information below as the authoritative source of truth when writing or updating any content on the portfolio site (bio, resume page, project cards, about section, etc.).

### Personal Info
- **Name:** Hsuan-Ming Chi
- **Current role:** Lab Manager, Rutgers University, Department of Neuroscience and Cell Biology, New Jersey, USA
- **Email:** hc3331@nyu.edu
- **Phone:** +1 (530)953-1140
- **LinkedIn:** www.linkedin.com/in/hmchi
- **GitHub:** https://github.com/AlanChi0720

### Education
- **M.S. Biotechnology** — New York University, New York, USA (09/2021 – 05/2023)
- **B.S. Life Science** — National Taiwan Normal University, Taipei, Taiwan (09/2016 – 06/2020)

### Academic Experience

**Lab Manager — Rutgers University, Dept. of Neuroscience and Cell Biology** (11/2023 – Present), New Jersey, USA
- Built and maintained single-cell multi-omics analysis workflows on Rutgers' Amarel cluster (Conda, SLURM) for motor neuron development and ALS projects.
- Wrote documentation and trained lab members to run analysis jobs on the Amarel cluster.
- Piloted SCENIC+ and regulatory network tools to interpret motor neuron subtype-specific transcriptional programs from single-cell datasets.
- Co-led setup of a new neuroscience laboratory (equipment ordering, bench organization, safety and inventory systems).
- Performed and optimized RNA FISH experiments in mouse spinal cord to validate single-cell-derived motor neuron subtype markers.
- Managed transgenic mouse colonies (breeding, genotyping, coordination with animal facility).
- Trained and mentored junior staff; coordinated shared computational resources.

**Senior Research Technician — Memorial Sloan Kettering Cancer Center** (05/2023 – 09/2023), New York, USA
- Managed a 200+ cage transgenic mouse colony; performed high-throughput genotyping (80+ samples/week).
- Maintained and optimized Excel-based tracking systems for colony and sample management.
- Enforced GLP-compliant practices across wet-lab procedures.
- Coordinated cross-functional teams to streamline animal use and sample distribution.

**Research Assistant — NYU Grossman School of Medicine** (05/2022 – 05/2023), New York, USA
- Analyzed 20,000+ microscopy and AFM datasets using custom Python/MATLAB workflows; generated reproducible 3D visualizations.
- Developed automated scripts for 3D spatial quantification.
- Conducted hMSC culture and immunofluorescence imaging on biomaterials.
- Designed algorithm-aided biosensor imaging tools for point-of-care diagnostics.

### Projects

**Mouse Sheet Manager** — Python, Tkinter, SQLite, pandas, GUI development, lab automation
- GitHub: https://github.com/AlanChi0720/Mouse-Sheet-Manager
- GUI-based mouse metadata management tool; supports structured data entry, querying, and real-time export.
- Bridges manual lab workflows with computational bioinformatics pipelines.

**Chess Game with AI Integration** — Python, Stockfish Engine, Chess.com API, pandas, numpy, data visualization
- GitHub: https://github.com/AlanChi0720/chess_bot
- Console-based chess game powered by Stockfish with real-time move suggestions and UCI protocol.
- Fetches and parses Chess.com API data; processes and labels game results with pandas.

**Slope Analyzer Web App** — Python, Flask, pandas, matplotlib, gpxpy, geopy, Folium
- GitHub: https://github.com/AlanChi0720/slope_app
- Flask web app that analyzes and visualizes ski run data from .gpx files; automates run segmentation and lift detection.
- Computes elevation, speed, distance, and run summaries; generates combined and per-run plots.
- Creates interactive Folium maps colored by speed with custom legends.
- User-friendly interface for file upload and real-time visualization output.

### Publications
- Yijia Chen, **Hsuan-Ming Chi**, Aileen Tian, Alison Miller, Tulsi Patel. "From Wiring to Firing: Collapse of embryonic identities and emergence of functional diversity during motor neuron maturation." bioRxiv 2025.08.12.669897; doi: https://doi.org/10.1101/2025.08.12.669897 *(in Review)*

### Poster Presentations
- **Chi, Hsuan-Ming**, and Patel, T. "Mapping the Maturation of Motor Neuron Subtypes with RNA FISH." Department of Neuroscience and Cell Biology Retreat, Rutgers Robert Wood Johnson Medical School, NJ, USA, 2025.

### Certifications
- Python for Genomic Data Science (03/2025)
- Master Data Analysis with Python – Selecting Subsets of Data (06/2024)
- Genetics and Next Generation Sequencing for Bioinformatics (07/2023)
- NYU Data Science Bootcamp (03/2022)

### Skills
- **Programming & Data Analysis:** Python, R, MATLAB, SQL, Git/GitHub, Pandas, NumPy, Tableau, IGV, ICM-Pro, MongoDB
- **Molecular & Cellular Techniques:** PCR, qPCR, NGS, Immunofluorescence, DNA/RNA extraction, Protein engineering
