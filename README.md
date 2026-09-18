# Knowledge Portal

Public presentation repository for artifacts explicitly published from the private `kewinall/knowledge-workspace` repository.

## Repository role

This repository is **public** and should contain only publishable material.

Generated website content lives in:

```text
site/
```

The `site/` directory is replaced automatically by the publishing workflow in `knowledge-workspace`. Do not use it as the source-of-truth for manual editing.

## Deployment flow

```text
knowledge-workspace
  html/publish/**
        |
        v
  build_portal.py
        |
        v
knowledge-portal/site
        |
        v
GitHub Pages
```

## GitHub Pages

Configure **Settings → Pages → Build and deployment → Source → GitHub Actions**.

After that, updates to `site/**` are deployed automatically by `.github/workflows/pages.yml`.
