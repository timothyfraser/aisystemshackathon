# Demo: ShinyApp Dashboard

This folder contains a minimal Shiny app template for the AI Systems Hackathon. You can extend it with inputs and outputs that call generative AI (e.g., OpenAI or Ollama) or display data from an API or database.

## Files

- `app.R` — Single-file Shiny app (UI + server). Replace or extend the histogram example with your own logic and AI calls.
- `workflow.R` — Optional script to test functions before wiring them into the app.
- `manifest.json` — Used by Posit Connect for deployment.

## Run locally

In R, open `app.R` and click **Run App**, or:

```r
shiny::runApp(".")
```

## Deploy

Deploy this folder to Posit Connect as a Shiny application (see [docs/resources.md](../../docs/resources.md) for deployment resources).
