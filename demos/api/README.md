# Demo: REST API with Plumber

This folder contains a minimal Plumber API template for the AI Systems Hackathon. You can extend it with endpoints that call generative AI (e.g., OpenAI or Ollama) or query a database.

## Files

- `plumber.R` — Defines API routes (e.g. `/echo`, `/plot`, `/sum`). Add your own routes and wire them to AI or data logic.
- `manifest.json` — Used by Posit Connect for deployment.

## Run locally

In R:

```r
library(plumber)
pr <- plumber::pr_run(plumber::pr("plumber.R"), port = 8000)
```

Then open `http://127.0.0.1:8000/docs` for the interactive API docs.

## Deploy

Deploy this folder to Posit Connect as an API (see [docs/resources.md](../../docs/resources.md) for deployment resources).
