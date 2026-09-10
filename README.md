# AI × Climate

A running review of artificial intelligence and machine learning in climate research.

## Local setup

Install [Quarto](https://quarto.org/docs/get-started/), then from this repository run:

```bash
quarto preview
```

This opens a local preview and automatically refreshes as you edit.

## Publish

The site is configured to publish automatically through GitHub Actions whenever a commit is pushed to `main`.

After creating the GitHub repository, go to:

**Settings → Pages → Build and deployment → Source → GitHub Actions**

Then every push to `main` will render and deploy the site.

## Add a new issue

Copy the issue template into a dated folder under `posts/`, for example:

```bash
mkdir -p posts/2026-09-state-of-ai-climate
cp templates/issue.qmd posts/2026-09-state-of-ai-climate/index.qmd
```

Update the YAML metadata, write the article, add citations to `references.bib`, then commit and push. Use `draft: true` in the article metadata while a piece should remain out of the rendered site.

Images and other article-specific files should live beside that article's `index.qmd`.

## Important configuration

The current repository/site name is assumed to be `ai-climate`, giving:

```text
https://evanwellmeyer.github.io/ai-climate/
```

If the repository is renamed, update both `website.site-url` and the GitHub navbar link in `_quarto.yml`.
