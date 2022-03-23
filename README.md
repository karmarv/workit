
[![pages-build-deployment](https://github.com/karmarv/workit/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/karmarv/workit/actions/workflows/pages/pages-build-deployment)

[https://karmarv.github.io/workit](https://karmarv.github.io/workit)

# Instructions for Author
A template for turning Jupyter notebooks and markdown files into a website.

Steps to use this template:

- Refer the materials theme docs for updates https://squidfunk.github.io/mkdocs-material/reference/data-tables/
- Add/remove python dependencies for notebook items in `requirements.txt` if need.
- Add folders (e.g., `chapter_01`) and files (e.g., `intro.ipynb`, `index.md`) to the `docs` folder.
- Open `mkdocs.yml` and make several changes, including `site_name`, `site_url`, `repo_url`, and `nav`. If you don't want the notebooks to be executed when building the website, set `execute: False` under `plugins`.
- Customize the issue template (`.github/ISSUE_TEMPLATE/config.yml`) if needed. 
- Commit and check out the website at https://karmarv.github.io/workit

## Setup Environment

### Conda 
- `conda create -n web`
- `conda activate web`
- `pip install -f requirements.txt`

### MkDocs
- Ensure all the plugins and themes are installed as per requirements file
- `mkdocs serve`
