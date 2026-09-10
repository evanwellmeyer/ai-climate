# One-time setup

## 1. Repository

The public repository is `evanwellmeyer/ai-climate`.

## 2. Push these files

From the directory containing this project:

```bash
git init
git add .
git commit -m "Initial Quarto site"
git branch -M main
git remote add origin https://github.com/evanwellmeyer/ai-climate.git
git push -u origin main
```

## 3. Enable GitHub Pages

In the GitHub repository:

**Settings → Pages → Build and deployment → Source → GitHub Actions**

The workflow in `.github/workflows/publish.yml` will render and deploy the site.

## 4. Work locally

On macOS, Quarto can be installed with:

```bash
brew install --cask quarto
```

Then preview the site with:

```bash
quarto preview
```

## Publishing future issues

Copy `templates/issue.qmd` into a new dated folder under `posts/`, edit it, and push to `main`.

```bash
git add .
git commit -m "Publish issue: <title>"
git push
```
