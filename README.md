# Diastology — LV Diastolic Function & LAP Estimator

A single-file, fully client-side tool that walks the ASE LV diastolic function &
left atrial pressure grading algorithm. No backend, no data leaves the browser.

## Files
- `index.html` — the entire app (HTML + CSS + JS inline)
- `netlify.toml` — static publish config (serves the repo root)

## Local use
Open `index.html` in any browser. That's it.

## Deploy (Netlify + GitHub auto-deploy)
This repo is linked to a Netlify site. Every push to `main` triggers a redeploy.

Update workflow:
```bash
# make your edits to index.html
git add index.html
git commit -m "describe the change"
git push
```
Netlify rebuilds and publishes in ~30 seconds.

## Scope / disclaimer
Clinical decision-support only. Standard cutoffs do not apply in the confounder
conditions listed in the app (MAC, MR, MS, AF, LVAD, non-cardiac PH, HTx,
pericardial constriction), which return an indeterminate result by design.
Clinical correlation and reader judgment govern.
