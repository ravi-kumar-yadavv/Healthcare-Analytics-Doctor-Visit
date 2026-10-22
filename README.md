# Healthcare Analytics for Doctor Visits

An exploratory data analysis (EDA) project using the AICTE–TIRTC student dataset to study patterns in doctor visits and how they vary across demographic, health, financial, and healthcare-support variables.

## Project Overview

- **Dataset:** Healthcare Analytics for Doctor Visits
- **Records:** 5,190
- **Original columns:** 13
- **Main outcome:** `visits` — number of doctor visits during the period covered by the dataset
- **Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

## Objectives

1. Inspect dataset structure and data quality.
2. Summarize the distribution of doctor visits.
3. Explore visit patterns by gender, recorded age and income values, illness, health, reduced activity, chronic-condition indicators, and healthcare-support indicators.
4. Present findings through clear charts and summary tables.
5. Document limitations and responsible interpretation.

## Repository Structure

```text
Healthcare_Analytics_Doctor_Visits/
├── Healthcare_Analytics_Doctor_Visits.ipynb
├── healthcare_doctor_visits.csv
├── README.md
└── requirements.txt
```

## Getting Started

### 1. Clone or download this repository

If using Git:

```bash
git clone <your-repository-url>
cd Healthcare_Analytics_Doctor_Visits
```

### 2. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `Healthcare_Analytics_Doctor_Visits.ipynb` and run the cells from top to bottom. Keep the CSV file in the same folder as the notebook.

## Analysis Included

- Dataset overview, data types, and descriptive statistics
- Missing-value, duplicate-row, and identifier checks
- Doctor-visit frequency distribution
- Gender and recorded age-level comparisons
- Recorded income-level distribution and relationship with visits
- Illness count and visit comparisons
- Recorded health values and reduced activity
- Chronic-condition indicators (`nchronic`, `lchronic`)
- Healthcare support indicators (`private`, `freepoor`, `freerepat`)
- Box plots, numeric correlation heatmap, and grouped summary table
- Dataset-generated key findings, conclusion, limitations, and further-work recommendations

## Column Notes

The accompanying dataset guide defines `visits` as the number of doctor visits during the period covered by the dataset. It describes `age` and `income` as numeric/level values but does not specify units or conversion rules. The direction of the `health` measure is also not documented in detail. This project therefore uses cautious labels such as “recorded value” rather than assuming units.

`Unnamed: 0` is treated as a record identifier and excluded from analytical charts/correlations.

## Important Limitations

- This is exploratory analysis, not a clinical tool.
- Observed differences and correlations do not prove cause and effect.
- The supplied guide does not fully specify the age/income units, health-score direction, sampling methodology, or the exact visit time window.
- Results may not generalize beyond this dataset.
- No diagnosis or individual treatment recommendations are made.

## Conclusion

This project demonstrates a complete beginner-friendly workflow for healthcare data analysis: loading and inspecting data, checking data quality, summarizing variables, creating visualizations, comparing groups, and writing evidence-based conclusions. The notebook calculates the specific findings directly from the included dataset.

## Acknowledgment

Prepared as a student learning project in the AICTE–TIRTC program context. Dataset descriptions are based on the supplied student dataset guide.
