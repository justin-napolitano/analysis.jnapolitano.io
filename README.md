# analysis.jnapolitano.io

A comprehensive collection of Jupyter Notebook-based analyses and documentation focused on political, legal, freight logistics, energy, and human rights topics. This repository contains scripts, notebooks, and resources to build, deploy, and back up the documentation website journal.jnapolitano.io.

---

## Features

- Automated build and deployment scripts for static site generation using Sphinx and Makefile.
- Dropbox integration for backing up generated HTML documentation.
- Diverse topical coverage including Supreme Court voting behavior, Kurdish conflict analysis, human rights law frameworks, and freight logistics.
- Rich documentation structure with articles, bibliography, and detailed project analyses.
- Uses Jupyter Notebooks with MyST Markdown for interactive and reproducible research.

---

## Tech Stack

- Primary Language: Jupyter Notebook (Python)
- Documentation: Sphinx with extensions like ablog, myst_nb, sphinx_copybutton, sphinx_design, sphinx_thebe
- Dropbox SDK for Python for backup automation
- Bash scripting for deployment and environment setup
- Makefile for build automation

---

## Getting Started

### Prerequisites

- Python 3.5 or higher
- pip package manager
- Dropbox account and API token for backup functionality

### Installation

1. Clone the repository:

```bash
git clone https://github.com/justin-napolitano/analysis.jnapolitano.io.git
cd analysis.jnapolitano.io
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. (Optional) For Rocky Linux or similar distributions:

```bash
pip install -r requirements_rocky.txt
```

### Build and Deploy

- Build the HTML documentation:

```bash
make html
```

- Deploy the site to GitHub Pages:

```bash
./deploy.sh
```

- Backup the generated HTML to Dropbox:

```bash
python3 backup_html.py
```

---

## Project Structure

```
analysis.jnapolitano.io/
├── acp.sh                 # Bash script (purpose assumed for automation)
├── backup_html.py         # Python script to back up HTML docs to Dropbox
├── chtml.sh               # Bash script (purpose assumed for HTML related tasks)
├── deploy.sh              # Bash script to deploy site to GitHub Pages
├── deployz.sh             # Another deployment script variant
├── doit.sh                # Bash script (purpose assumed for task automation)
├── install.sh             # Bash script for environment setup
├── label_list.py          # Script to read and display labels from Sphinx pickle files
├── Makefile               # Build automation file
├── pullit.sh              # Bash script for git pull
├── pushit.sh              # Bash script for git push
├── python_build.py        # Python script to automate build pipeline
├── requirements.txt       # Python dependencies
├── requirements_rocky.txt # Python dependencies for Rocky Linux
├── requirments.txt        # (Likely typo, duplicate requirements)
├── source/                # Documentation source files (Markdown, conf.py, TOC)
├── todo/                  # TODO notes and plans
└── uninstall.sh           # Bash script to uninstall environment
```

---

## Future Work / Roadmap

- Improve documentation coverage and add more detailed README sections.
- Automate testing and continuous integration for build and deployment.
- Enhance backup system with incremental backups and error handling.
- Expand topical analyses with more datasets and interactive visualizations.
- Refactor scripts for better modularity and error resilience.

---

*Note: Some scripts and files have limited inline documentation; users are encouraged to review and adapt them as needed.*
