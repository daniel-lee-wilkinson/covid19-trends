# COVID-19 Data Analysis
## Testing Rates and Positive Cases: January–June 2020

An R Quarto report analysing COVID-19 testing rates and positive cases across the top ten most-tested countries between January and June 2020. Uses time-series visualisation and population-adjusted ranking to show that high positive-to-tested ratios reflect testing strategy constraints rather than true disease burden.

## Research Questions

1. Which countries reported the highest number of deaths due to COVID-19?
2. Which countries had the highest ratio of positive cases to tests conducted?
3. Which countries made the best testing effort relative to their population?
4. Which countries were most and least affected relative to their population?

## Data

Loaded directly from `https://dq-content.s3.amazonaws.com/505/covid19.csv` — no local files needed. Derived from Kaggle, provided by Dataquest. Covers 20 January to 1 June 2020.

## Key Findings

- The **UK, US, and Turkey** had the highest positive-to-tested ratios, but time-series analysis shows this reflects early testing being restricted to the most severe cases rather than higher infection rates
- **Italy** peaks earliest and falls fastest, consistent with being the first European country seriously hit
- **Australia** stays near 0% throughout, reflecting aggressive early containment
- **Italy** was most affected per capita; **India** least affected

## Requirements

- R 4.0+
- Quarto
- R packages: `tidyverse`, `skimr`, `readr`, `ggthemes`, `zoo`

```r
install.packages(c("tidyverse", "skimr", "readr", "ggthemes", "zoo"))
```

## Setup

1. Clone the repository
2. Open `report.qmd` in RStudio
3. Click **Render** to produce the PDF

No local data files required — the dataset loads from a URL.

## Project Structure

```
├── report.qmd     # Main Quarto report
└── .gitignore
```