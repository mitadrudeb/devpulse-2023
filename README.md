# DevPulse 2023 — Stack Overflow Developer Survey Analysis

This is my capstone project for the IBM Data Analytics Professional Certificate. The goal was to analyze the Stack Overflow Developer Survey 2023 dataset and find meaningful insights about what technologies developers are using today and what they plan to use in the future.

---

## What this project is about

The Stack Overflow Developer Survey is one of the largest surveys of software developers in the world. The 2023 edition had responses from 65,437 developers across 180+ countries.

I wanted to answer three questions from this data:

1. What programming languages, databases, and tools are developers actively using right now?
2. What technologies are they planning to learn or switch to next year?
3. Who are these developers — how old are they, where are they from, what's their education background?

---

## What I found

A few things surprised me during the analysis:

- JavaScript has been the most used language for years and it's still #1 — both in current use (37,492 respondents) and future demand (21,869). I expected Python to be closer.
- PostgreSQL is overtaking MySQL in future demand. MySQL is still the most used database today (26,245) but PostgreSQL is what more developers *want* to use next year (24,005). I thought MySQL would hold its position longer.
- Kubernetes jumped from #7 in current platform usage to #3 in desired platforms. Cloud-native development is clearly accelerating faster than I expected.
- 37% of all respondents are in the 25–34 age group, and 68% have at least a bachelor's degree. The developer community is younger and more formally educated than I assumed going in.

---

## Project structure

```
devpulse-2023/
├── notebooks/          — 14 Jupyter notebooks covering the full analysis pipeline
├── dashboard/          — Interactive dashboard built with Chart.js (open in browser)
├── data/
│   ├── processed/      — Cleaned datasets used in analysis
│   └── raw/            — Original source files (too large for GitHub, see data/README.md)
├── report/             — Final presentation PDF (submitted for grading)
├── requirements.txt
└── README.md
```

---

## The notebooks

I split the work across 14 notebooks, roughly following the course module structure:

| Notebook | What it covers |
|----------|----------------|
| 01_data_exploration | First look at the dataset — shape, columns, data types |
| 02_data_wrangling | Handling missing values, splitting pipe-delimited columns, removing duplicates |
| 03_exploratory_analysis | Frequency counts, top-10 rankings for all tech categories |
| 04_distribution_analysis | Statistical distributions across key columns |
| 05_outliers_duplicates | IQR-based outlier detection and removal |
| 06_correlation_analysis | Correlation matrix and heatmaps |
| 07_visualization_basics | Building the core chart types |
| 08_histogram_charts | Distribution histograms |
| 09_boxplot_analysis | Box plots for age and experience |
| 10_scatter_trendline | Scatter plots with regression lines |
| 11_pie_charts | Demographic breakdowns (age, employment, education) |
| 12_stacked_charts | Age vs education stacked bar analysis |
| 13_line_charts | Education level line chart |
| 14_bar_charts | Age group bar charts with filters |

---

## The dashboard

The dashboard is a single HTML file that runs entirely in the browser — no setup needed. It has three tabs:

- **Current Technology Usage** — languages, databases, platforms, and frameworks developers use today
- **Future Technology Trends** — what they want to work with next year
- **Demographics** — age, employment, country, education, and coding activities

To open it, just download the file and open it in Chrome or Firefox:
```
dashboard/StackOverflow_Dashboard.html
```

---

## How to run the notebooks

```bash
git clone https://github.com/mitadrudeb/devpulse-2023.git
cd devpulse-2023
pip install -r requirements.txt
jupyter notebook notebooks/
```

Note: The raw dataset is not included in this repo because it's too large for GitHub (~150MB). You can download it from the [Stack Overflow survey page](https://insights.stackoverflow.com/survey) or through the IBM Skills Network.

---

## Tools used

- Python 3.11
- pandas, numpy
- matplotlib, seaborn
- Jupyter Notebook
- Chart.js (for the dashboard)
- SQLite (for some of the SQL-based exercises)
- AI coding assistants (Claude, ChatGPT) — used occasionally for debugging errors and understanding concepts I was stuck on

---

## Results

The final presentation PDF is in the `report/` folder. It was graded as part of the IBM Data Analytics Professional Certificate capstone and scored 14/14.

---

## Data source

Stack Overflow (2023). Annual Developer Survey.
Available at: https://insights.stackoverflow.com/survey

The data is provided under the [Open Database License (ODbL)](https://opendatacommons.org/licenses/odbl/).

---

## About

I'm Mitadru Deb— currently building my skills in data analytics. This is one of the first end-to-end projects I've completed independently, from raw data all the way to a final report and interactive dashboard.

Feel free to connect on [LinkedIn](https://linkedin.com/in/mitadrudeb) if you have questions or feedback about the project.
