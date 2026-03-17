# Data Directory

## Structure

```
data/
├── raw/            ← Original source files (NOT tracked in git — see below)
└── processed/      ← Cleaned & transformed files (tracked in git)
```

---

## Raw Data (not included in this repo)

The raw survey file is ~150MB and exceeds GitHub's recommended limits.

**To reproduce this project from scratch, download:**

| File | Source | Size |
|------|--------|------|
| `survey_data_updated.csv` | IBM Skills Network / Stack Overflow 2023 | ~150MB |
| `survey-data.sqlite` | IBM Skills Network | ~200MB |
| `survey-results-public.sqlite` | Stack Overflow Public | ~200MB |

**Download links:**
- Stack Overflow Survey: https://insights.stackoverflow.com/survey
- IBM Skills Network: Available via the IBM Data Science Professional Certificate on Coursera

Place downloaded files in `data/raw/` before running the notebooks.

---

## Processed Data (included)

These cleaned/transformed files are small enough to track directly:

| File | Description | Rows |
|------|-------------|------|
| `survey_data_cleaned.csv` | After null handling and deduplication | ~65,000 |
| `survey_data_analyzed.csv` | With computed columns and rankings | ~65,000 |
| `survey_data_distribution_analysis.csv` | Distribution stats per column | varies |
| `survey_data_correlation_analysis.csv` | Correlation matrix output | varies |
| `survey_data_no_outliers.csv` | After IQR-based outlier removal | ~62,000 |
