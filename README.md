# AI for Life-Science Professionals · CityUx Labs

**Prototype.** Free, hands-on browser labs that teach AI to people who work in life sciences: scientists, lab staff, and biotech and health professionals. A CityUx project from City University of Seattle.

**Live site:** https://clarkngo.github.io/cityux-ai-life-sciences/

## Labs

| Lab | What you do |
|---|---|
| [1 · Protein Structure Explorer](labs/protein-explorer.html) | Compare a lab-measured protein (PDB) with AlphaFold's prediction and read its pLDDT confidence. |
| [2 · Assay Hit Predictor](labs/assay-simulator.html) | Train a k-nearest-neighbors model on simulated screening data and watch it overfit. |
| [3 · Literature Triage Agent](labs/literature-triage.html) | Check a rule-based agent's screening of ten fictional abstracts, and measure its precision and recall. |
| [4 · Can This Data Cross the Border?](labs/data-border.html) | Eight US–China data-sharing scenarios: share, review first, or don't share. |

## Design rules

- **Static and free.** Plain HTML, CSS, and JavaScript on GitHub Pages. No build step, no backend, no accounts, no API keys.
- **Methods, not sensitive data.** Only public datasets (fetched live) or synthetic and fictional data. Never patient, genetic, or company data.
- **Accessible.** Aim for WCAG 2.2 AA: keyboard-usable controls, `aria-pressed` toggles, text summaries for every chart.
- **CityU brand.** Marine `#002D5C`, Blood Orange `#F63E02` accent, Teal `#3BBABD` secondary; Open Sans.

## Status and open items

- Not yet reviewed by a life-science domain expert. A reviewer from a partner's pharmacy or food-biotech program, or from CityU's health side, should check Labs 1–3.
- Lab 4 simplifies legal rules for teaching and is not legal advice. Have it reviewed by a compliance or export-control office before wider use.
- May later be embedded in Open edX as part of a CityUx micro-credential.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000. Lab 1 needs an internet connection to fetch structures.

## License

Content CC BY 4.0, code MIT. See [LICENSE.md](LICENSE.md).
