# 🚀 DevPulse 2023 — Decoding the Global Developer Ecosystem

[![IBM Data Science](https://img.shields.io/badge/IBM-Data%20Science%20Certificate-054ADA?style=flat&logo=ibm)](https://www.coursera.org/professional-certificates/ibm-data-science)
[![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=flat&logo=python&logoColor=white)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter&logoColor=white)](https://jupyter.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Capstone project for the IBM Data Analytics Professional Certificate.**  
> A full end-to-end data analysis of the Stack Overflow Developer Survey 2023 — covering data wrangling, exploratory analysis, statistical analysis, visualization, dashboard design, and findings reporting.

---

## 📌 Project Overview

**DevPulse 2023** analyzes responses from **65,437 developers across 180+ countries** to answer three core questions:

1. 🔧 **What technologies are developers using right now?**
2. 📈 **What technologies are they planning to adopt next year?**
3. 👥 **Who are the developers — demographically?**

The findings reveal actionable insights for developers, recruiters, educators, and tech leaders about the current state and near-future trajectory of the global software ecosystem.

---

## 🗂️ Repository Structure

```
devpulse-2023/
│
├── 📓 notebooks/                    # Jupyter analysis notebooks (M1–M15)
│   ├── 01_data_exploration.ipynb    # Initial data loading and survey structure
│   ├── 02_data_wrangling.ipynb      # Cleaning, nulls, duplicates, normalization
│   ├── 03_exploratory_analysis.ipynb# Frequency distributions, top-10 rankings
│   ├── 04_distribution_analysis.ipynb # Statistical distributions
│   ├── 05_outliers_duplicates.ipynb # Outlier detection and removal
│   ├── 06_correlation_analysis.ipynb# Correlation heatmaps and analysis
│   ├── 07_visualization_basics.ipynb# Core chart building
│   ├── 08_histogram_charts.ipynb    # Distribution histograms
│   ├── 09_boxplot_analysis.ipynb    # Box plots for age/salary distributions
│   ├── 10_scatter_trendline.ipynb   # Scatter plots with trend lines
│   ├── 11_pie_charts.ipynb          # Demographic pie charts
│   ├── 12_stacked_charts.ipynb      # Age × Education stacked analysis
│   ├── 13_line_charts.ipynb         # Education level line chart
│   └── 14_bar_charts.ipynb          # Age group bar chart analysis
│
├── 📊 dashboard/
│   └── StackOverflow_Dashboard.html # Interactive Chart.js dashboard (3 tabs, 12 charts)
│
├── 📁 data/
│   ├── raw/                         # Original source data (see note below)
│   └── processed/                   # Cleaned and transformed datasets
│       ├── survey_data_cleaned.csv
│       ├── survey_data_analyzed.csv
│       ├── survey_data_distribution_analysis.csv
│       ├── survey_data_correlation_analysis.csv
│       └── survey_data_no_outliers.csv
│
├── 📄 report/
│   └── Data_Analyst_Capstone_Project_Report.pdf  # Final 14-slide presentation
│
├── requirements.txt                 # Python dependencies
├── .gitignore
└── README.md
```

> **Note on raw data:** The original `survey_data_updated.csv` (65,437 rows) exceeds GitHub's recommended file size. Download it directly from [Stack Overflow's public survey data](https://insights.stackoverflow.com/survey) or the IBM Skills Network.

---

## 📊 Dashboard Preview

The interactive dashboard is built with **Chart.js** and runs entirely in the browser — no server needed.

**Open `dashboard/StackOverflow_Dashboard.html` in any modern browser.**

### Tab 1 — Current Technology Usage
| Chart | Type | Key Finding |
|-------|------|-------------|
| Top 10 Languages | Horizontal Bar | JavaScript leads (37,492 users) |
| Top 10 Databases | Column Chart | MySQL most used (26,245) |
| Top 10 Platforms | Word Cloud | Linux dominant (30,522) |
| Top 10 Web Frameworks | Hierarchy Bubble | React #1 (25,029) |

### Tab 2 — Future Technology Trends
| Chart | Type | Key Finding |
|-------|------|-------------|
| Languages Desired | Horizontal Bar | JavaScript still #1 (21,869) |
| Databases Desired | Column Chart | PostgreSQL surges to #1 (24,005) |
| Platforms Desired | Tree Map | Kubernetes jumps from #7 → #3 |
| Frameworks Desired | Hierarchy Bubble | Next.js fastest-growing |

### Tab 3 — Demographics
| Chart | Type | Key Finding |
|-------|------|-------------|
| Age Distribution | Pie Chart | 25–34 dominant (37%) |
| Employment Status | Pie Chart | 67% employed full-time |
| Country Distribution | Map Chart | US + India = 29% |
| Education Level | Pie Chart | 68% bachelor's degree+ |
| Coding Activities | Pie Chart | Hobby coding leads (33,241) |

---

## 🔍 Key Findings

### 💻 Languages
- **JavaScript** tops both current (37,492) and desired (21,869) usage — unmatched end-to-end dominance
- **Python** surges to #2 desired, driven by AI/ML demand
- **Rust** enters the desired top-6 despite low current adoption — a major emerging signal
- **TypeScript** holds #5 in both charts — type safety is now a baseline expectation

### 🗄️ Databases
- **PostgreSQL** overtakes MySQL in future demand (24,005 vs 12,269) — the most significant technology shift in the survey
- **SQLite** is underrated at #3 in both charts — embedded/edge computing demand is real
- **Neo4j** and **Cassandra** enter the desired top-10 — graph and distributed DBs are gaining momentum

### ☁️ Platforms & Frameworks
- **Linux + Docker + Kubernetes** = the default production stack
- **Kubernetes** jumps from #7 current → #3 desired — cloud-native is accelerating
- **React + Node.js** hold dual #1/#2 in both current and desired frameworks

### 👥 Demographics
- **25–34** age cohort: 37% of all developers (industry's primary career-builders)
- **67%** employed full-time; independent contracting at 5.4%
- **68%** hold at least a bachelor's degree
- **US + India** represent ~29% of respondents — Asia's trajectory is upward

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Python 3.11** | Core analysis language |
| **pandas** | Data wrangling and manipulation |
| **numpy** | Numerical operations |
| **matplotlib** | Static visualizations |
| **seaborn** | Statistical plotting |
| **sqlite3** | Database querying |
| **Jupyter Notebook** | Interactive analysis environment |
| **Chart.js v4.4** | Interactive dashboard (browser-native) |
| **HTML / CSS / JS** | Dashboard frontend (zero dependencies) |

---

## ⚡ Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/devpulse-2023.git
cd devpulse-2023
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter
```bash
jupyter notebook notebooks/
```

### 4. Open the dashboard
```bash
# Simply open in your browser:
open dashboard/StackOverflow_Dashboard.html
# or on Windows:
start dashboard/StackOverflow_Dashboard.html
```

---

## 📁 Notebook Guide

| Notebook | Module | Description |
|----------|--------|-------------|
| `01_data_exploration.ipynb` | M1 | Load dataset, inspect shape, columns, dtypes |
| `02_data_wrangling.ipynb` | M2 | Handle missing values, normalize multi-select columns |
| `03_exploratory_analysis.ipynb` | M3 | Frequency distributions, top-10 rankings |
| `04_distribution_analysis.ipynb` | M4 | Statistical distributions and normality checks |
| `05_outliers_duplicates.ipynb` | M5 | Outlier detection (IQR), duplicate removal |
| `06_correlation_analysis.ipynb` | M6 | Correlation matrix, heatmaps |
| `07_visualization_basics.ipynb` | M7 | Core visualization patterns |
| `08_histogram_charts.ipynb` | M8 | Distribution histograms with outlier handling |
| `09_boxplot_analysis.ipynb` | M9 | Box plots for age and compensation analysis |
| `10_scatter_trendline.ipynb` | M10 | Scatter plots with regression trend lines |
| `11_pie_charts.ipynb` | M12 | Demographic pie charts (age, employment, education) |
| `12_stacked_charts.ipynb` | M13 | Age × Education stacked bar analysis |
| `13_line_charts.ipynb` | M14 | Education level line chart with markers |
| `14_bar_charts.ipynb` | M15 | Age group bar chart with filters |

---

## 📈 Results Summary

```
Dataset:     Stack Overflow Developer Survey 2023
Rows:        65,437 respondents
Columns:     114 attributes
Countries:   180+ represented
Notebooks:   14 analysis modules
Charts:      12 dashboard visualizations
Tabs:        3 (Current Tech · Future Trends · Demographics)
Report:      14-slide PDF presentation
Final Grade: 100% ✅
```

---

## 🏆 Certification

This project was completed as the **capstone for the IBM Data Analytics Professional Certificate** on Coursera.

- ✅ Final grade: **100% (14/14 points)**
- ✅ Certificate: IBM Data Analytics Professional Certificate
- ✅ Skills validated: Data wrangling · EDA · Statistical analysis · Data visualization · Dashboard design · Findings reporting

---

## 📄 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.

The Stack Overflow Developer Survey data is provided under the [Open Database License (ODbL)](https://opendatacommons.org/licenses/odbl/).

---

## 🙋 About

**[Your Name]**  
Data Analyst | IBM Certified  
📧 [your.email@example.com]  
💼 [linkedin.com/in/yourprofile]  
🐙 [github.com/your-username]

---

*Built with Python, Jupyter, Chart.js, and a lot of curiosity about the developer ecosystem.*
