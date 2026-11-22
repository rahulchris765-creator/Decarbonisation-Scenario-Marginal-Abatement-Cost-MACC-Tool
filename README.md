# Decarbonisation Scenario & Marginal Abatement Cost (MACC) Tool

Models the cost-effectiveness of a set of decarbonisation measures — capex, annual savings and carbon abatement — and ranks them into a marginal abatement cost curve, the way a client-facing engagement would prioritise "right-sized" recommendations rather than a flat list of options.

**[Live demo →](https://rahulchris765-creator.github.io/projects/decarbonization-macc-tool.html)**

## Why I built this

Clients don't need every possible decarbonisation measure recommended at once — they need the ones that make sense for their budget and payback horizon, in order. This tool applies marginal-abatement-cost logic (the same approach behind McKinsey-style MACC curves) to real retrofit measure economics, to practice turning a list of options into a prioritised, defensible recommendation.

## What it does

- Editable table of decarbonisation measures (LED lighting, insulation, smart heating controls, air-source heat pumps, solar PV, EV fleet transition), each with:
  - Capex per site
  - Expected lifetime
  - Annual opex saving
  - Annual carbon abatement
  - Number of sites
- Annualises capex using a capital recovery factor, nets it against annual savings, and ranks every measure by **£ per tonne of CO2e abated**
- Renders an interactive marginal abatement cost curve: bar width = abatement potential, bar height = cost per tonne, colour-coded net-cost-saving vs. net-cost
- Surfaces a plain-language recommendation: which measures pay for themselves and should be funded first, and how much abatement that unlocks at zero or negative net cost
- All inputs are editable — model a different building stock, site count, or local cost base

## Methodology

Default measures and costs are generalised from the economics of UK domestic retrofit programmes (ECO4/GBIS) I've delivered as a Project Manager, simplified into illustrative per-site figures. Capex is annualised at a 6% discount rate assumption. For illustration only — a real client recommendation would use site-specific surveys and current local cost data.

## Tech stack

Plain HTML, CSS and JavaScript, with the chart hand-drawn in SVG — no build step, no dependencies, no charting library.

## Disclaimer

This is a self-directed portfolio project. It is not audited and should not be used as the basis for an actual investment or procurement decision without independent verification of every cost and savings assumption.

## Author

**Rahul Christhuraj Latharani** — [Portfolio](https://rahulchris765-creator.github.io/) · [LinkedIn](https://linkedin.com/in/rahul-christhuraj)
