---
slug: "github-analysis.jnapolitano.io"
title: "analysis.jnapolitano.io"
repo: "justin-napolitano/analysis.jnapolitano.io"
githubUrl: "https://github.com/justin-napolitano/analysis.jnapolitano.io"
generatedAt: "2025-11-23T08:12:18.063929Z"
source: "github-auto"
---


# Behind the Scenes of analysis.jnapolitano.io: A Personal Journey into Data-Driven Research and Documentation

Hey there! I'm Justin Napolitano, and I want to share a bit about my project repository, **analysis.jnapolitano.io**. This repository is more than just code—it's a living archive of my research, analysis, and documentation efforts across a variety of fascinating topics including political science, law, freight logistics, energy, and human rights.

## Motivation

I've always been passionate about using data and computational tools to understand complex social and political phenomena. Whether it's analyzing Supreme Court voting behavior, exploring the Kurdish conflict in Anatolia, or mapping freight logistics networks, I wanted a centralized place to develop, document, and share my work. 

This project serves as the backbone for my public-facing website, journal.jnapolitano.io, where I publish articles, analyses, and interactive content. The goal is to make rigorous research accessible and reproducible.

## What Problem Does This Solve?

Research projects often end up fragmented—data here, scripts there, documentation scattered across platforms. This repository tackles that by providing an integrated environment for:

- Writing and executing Jupyter Notebooks enriched with MyST Markdown for rich text and code.
- Building a static website with Sphinx, complete with blog posts, bibliographies, and detailed project documentation.
- Automating deployment to GitHub Pages and backing up the generated site to Dropbox.
- Managing dependencies and build pipelines with Python scripts and Makefiles.

This setup not only streamlines my workflow but also ensures that my research outputs are well-structured, version-controlled, and easy for others to explore.

## How It's Built

At its core, the repository uses **Jupyter Notebooks** for interactive data analysis and storytelling. These notebooks are converted into static HTML pages using **Sphinx** with a rich set of extensions like `ablog` for blogging, `myst_nb` for notebook support, and others that enhance usability and presentation.

The build process is automated with a **Makefile** and Python scripts (`python_build.py`) that handle tasks like cleaning old builds, installing dependencies, and running the site build. Deployment scripts (`deploy.sh`) publish the site to GitHub Pages, while `backup_html.py` uses the Dropbox API to back up the site remotely—because losing work is not an option!

I also use several Bash scripts to manage git operations (`pullit.sh`, `pushit.sh`) and environment setup (`install.sh`, `uninstall.sh`). This combination of tools lets me focus on research while keeping the infrastructure robust and repeatable.

## Interesting Implementation Details

- The **Dropbox backup script** is tailored to upload the entire built HTML directory, using the Dropbox Python SDK. It handles errors like insufficient space gracefully, ensuring backups don't silently fail.

- The **build pipeline** in `python_build.py` orchestrates multiple steps: cleaning previous builds, generating HTML, adding changes, committing with timestamps, and pushing to remote. This encapsulation reduces manual overhead.

- The documentation source includes **rich content** such as bibliographies, legal frameworks, and interactive maps (e.g., freight logistics GIS data visualized with geopandas and folium).

- The project embraces reproducible research principles by integrating code, data, and narrative in one place.

## Why this project matters for my career

This repository represents my commitment to rigorous, transparent, and impactful research. By mastering tools like Jupyter, Sphinx, and automated deployment, I've built a portfolio that showcases not just my analytical skills but also my ability to communicate complex ideas effectively.

Maintaining this project sharpens my software engineering practices, especially in automation, documentation, and data management. These skills are invaluable whether I pursue academia, data science, or policy analysis.

Moreover, sharing my work publicly invites collaboration and feedback, opening doors to new opportunities and connections in the research community.

---

Thanks for reading! If you're interested in any of the topics or tools I use, feel free to explore the repository or reach out.
