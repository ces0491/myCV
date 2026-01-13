# myCV

Built with [Quarto](https://quarto.org/) and deployed to GitHub Pages.

**View my CV here:** [https://ces0491.github.io/myCV/](https://ces0491.github.io/myCV/)

## Overview

This repository contains the source files for a web-based CV/resume. The CV is written in Quarto Markdown (`.qmd`) with embedded R code for dynamic content, styled with custom CSS, and automatically rendered and deployed via GitHub Actions.

## Tech Stack

- **Quarto** - Document authoring and rendering
- **R** - Dynamic content generation (e.g., calculating years of experience)
- **GitHub Actions** - CI/CD for automatic rendering and deployment
- **GitHub Pages** - Hosting

## Project Structure

```
myCV/
├── myCV.qmd           # Main CV content (Quarto markdown)
├── _quarto.yml        # Quarto project configuration
├── style.css          # Custom styling
├── back-to-top.html   # Back-to-top button component
├── index.html         # Rendered output (generated)
└── .github/
    └── workflows/
        └── quarto.yml # GitHub Actions workflow
```

## Local Development

### Prerequisites

- [Quarto CLI](https://quarto.org/docs/get-started/)
- [R](https://www.r-project.org/) (with `knitr` and `rmarkdown` packages)

### Render Locally

```bash
quarto render myCV.qmd --to html
```

## Deployment

The CV is automatically rendered and deployed to GitHub Pages when changes are pushed to the `main` branch. The GitHub Actions workflow:

1. Sets up Quarto and R
2. Installs required R packages
3. Renders `myCV.qmd` to HTML
4. Deploys to GitHub Pages

## License

This project contains personal information and is provided for reference purposes.
