---
slug: github-analysis-jnapolitano-io-note-technical-overview
id: github-analysis-jnapolitano-io-note-technical-overview
title: analysis.jnapolitano.io
repo: justin-napolitano/analysis.jnapolitano.io
githubUrl: https://github.com/justin-napolitano/analysis.jnapolitano.io
generatedAt: '2025-11-24T18:30:25.740Z'
source: github-auto
summary: >-
  This repo hosts Jupyter Notebooks for various analyses covering political,
  legal, energy, and human rights topics. It's designed to build, deploy, and
  back up the documentation site at journal.jnapolitano.io.
tags: []
seoPrimaryKeyword: ''
seoSecondaryKeywords: []
seoOptimized: false
topicFamily: null
topicFamilyConfidence: null
kind: note
entryLayout: note
showInProjects: false
showInNotes: true
showInWriting: false
showInLogs: false
---

This repo hosts Jupyter Notebooks for various analyses covering political, legal, energy, and human rights topics. It's designed to build, deploy, and back up the documentation site at journal.jnapolitano.io.

## Key Features

- Uses Jupyter Notebooks with MyST Markdown for reproducible research.
- Automates builds with Sphinx and Makefile for static site generation.
- Backs up documentation to Dropbox.
- Topics include Supreme Court voting, Kurdish conflict, and freight logistics.

## Getting Started

1. Clone the repo:

    ```bash
    git clone https://github.com/justin-napolitano/analysis.jnapolitano.io.git
    cd analysis.jnapolitano.io
    ```

2. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Build the HTML:

    ```bash
    make html
    ```

4. Deploy to GitHub Pages:

    ```bash
    ./deploy.sh
    ```

Be aware: You'll need a Dropbox account and API token for backups.
