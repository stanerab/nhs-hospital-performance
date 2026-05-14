# NHS Hospital Performance – Elective 18-Week Standard

This project compares elective waiting-time performance for **Northumbria Healthcare NHS Foundation Trust** and **University Hospitals Birmingham NHS Foundation Trust**, benchmarked against the national average using monthly data published by NHS England.

The NHS operational standard requires that **92% of patients on an incomplete elective pathway should wait no more than 18 weeks** from referral to treatment. The aim of this project is to see how each trust performs over time and how they stack up against the national average.

## 🔗 Live Dashboard

https://stanerab.github.io/nhs-hospital-performance/

## What's Included

- **Cleaned dataset** combining the two trusts and the national figures
- **Trend charts** showing monthly performance over time
- **Gap-vs-national chart** showing how far each trust sits above or below the national average
- **Yearly performance comparison** for a year-on-year side-by-side view
- **HTML dashboard** bringing everything together

## Repository Contents

| File | Description |
| --- | --- |
| `Birmingham-Elective-proportion-waiting-withi....csv` | Raw NHS England data for University Hospitals Birmingham |
| `Northumbria-Elective-proportion-waiting-withi....csv` | Raw NHS England data for Northumbria Healthcare |
| `nhs_hospital_comparison_clean.csv` | Cleaned and merged dataset used for the analysis |
| `trend_comparison.png` | Monthly RTT performance trend for both trusts |
| `gap_vs_national.png` | Each trust's gap vs the national average |
| `yearly_comparison.png` | Yearly performance comparison |
| `index.html` | Dashboard bringing the charts together (served via GitHub Pages) |

## Tools

- **Python** – `pandas` for data cleaning, `matplotlib` for the charts
- **HTML / CSS** – dashboard layout and styling

The data cleaning and chart generation were done locally in Python; only the cleaned dataset, chart images, and the dashboard HTML are committed to the repo.

## Data Source

Monthly Referral to Treatment (RTT) waiting-time statistics published by NHS England:
<https://www.england.nhs.uk/statistics/statistical-work-areas/rtt-waiting-times/>

## Viewing Locally

```bash
git clone https://github.com/stanerab/nhs-hospital-performance.git
cd nhs-hospital-performance
```

Open `index.html` in any modern browser to view the dashboard.

## License

Released under the MIT License. NHS England data is published under the [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).

## Author

**Stan** (https://github.com/stanerab)
