# NHS Hospital Performance – Elective 18-Week Standard

This project compares elective waiting-time performance for **Northumbria Healthcare NHS Foundation Trust (RTF)** and **University Hospitals Birmingham NHS Foundation Trust (RRK)**, benchmarked against the England national average using monthly data published by NHS England.

The NHS operational standard requires that **92% of patients on an incomplete elective pathway should wait no more than 18 weeks** from referral to treatment. The aim of this project is to see how each trust performs over time and how they stack up against the national average.

## 🔗 Live Dashboard

**[stanerab.github.io/nhs-hospital-performance](https://stanerab.github.io/nhs-hospital-performance/)**

## Key Findings

Based on monthly data from late 2024 to September 2025:

- **Neither trust meets the 92% standard** — and neither does the national average (~62%). The gap between current reality and the operational target is the biggest story in the data.
- **Northumbria consistently outperforms the national average by ~20 percentage points**, holding steady around 80% throughout the period (latest: **82.6%**).
- **Birmingham sits below the national average**, running ~7–10 points behind for most of the period before climbing sharply from mid-2025 onwards (latest: **59.0%** vs national **61.8%**).
- **Yearly averages** are stable for Northumbria (~80% in both 2024 and 2025) and slightly improving for Birmingham (51% → 53%).

## What's Included

- **Cleaned dataset** combining both trusts and the national figures
- **Trend chart** showing monthly performance over time for both trusts and the national average
- **Gap-vs-national chart** showing how far each trust sits above or below the national line
- **Yearly performance comparison** for a smoothed year-on-year view
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

## What I Learned

- Half the project was getting the data into shape; the other half was choosing the right way to compare it.
- Cleaning matters, but the analytical choices what to compare, against what benchmark, over what timeframe matter just as much.
- A single trust's number only makes sense against a benchmark.
- A gap chart tells a sharper story than a trend chart.
- Pandas + matplotlib was more than enough for a project this size.
- A simple HTML dashboard on GitHub Pages turns a folder of charts into something shareable.

## License

Released under the MIT License. NHS England data is published under the [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).

## Author

Stanley Erhabor
https://github.com/stanerab
