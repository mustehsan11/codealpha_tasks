#  Unemployment Analysis in India — COVID-19 Impact

> **Data Science Internship — Task 2**  
> Exploratory data analysis and visualisation of unemployment trends across Indian states, with a focus on the impact of the COVID-19 pandemic.

---

##  Overview

This project analyses monthly unemployment data across Indian states from **May 2019 to November 2020**. It investigates how the COVID-19 lockdown affected employment, compares urban vs rural trends, identifies the worst-hit states, and surfaces seasonal patterns — all to inform evidence-based economic policy.

---

##  Project Structure

```
unemployment-analysis/
│
├── Unemployment_Analysis.ipynb        # Main Colab notebook
├── Unemployment_in_India.csv          # Dataset 1 — state-level (May 2019–Jun 2020)
├── Unemployment_Rate_upto_11_2020.csv # Dataset 2 — extended timeline (Jan–Nov 2020)
└── README.md
```

---

##  Dataset

| Field | Description |
|-------|-------------|
| `Region` | Indian state / union territory |
| `Date` | Month-end date |
| `Estimated Unemployment Rate (%)` | % of labour force unemployed |
| `Estimated Employed` | Number of employed persons |
| `Estimated Labour Participation Rate (%)` | % of working-age population in labour force |
| `Area` | Rural or Urban |

**Source:** [CMIE (Centre for Monitoring Indian Economy)](https://www.cmie.com/)  
**Records:** ~740 rows across 28 states and UTs

---

##  Tech Stack

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading, cleaning, manipulation |
| `numpy` | Numerical operations |
| `matplotlib` | Base plotting |
| `seaborn` | Statistical visualisations |
| `scipy` | Smooth curve interpolation |

---

##  Workflow

```
Load CSVs → Clean & Parse Dates → Feature Engineering
    → EDA & Statistics → 7 Visualisations → Insights & Policy Recommendations
```

---

##  Visualisations Included

| # | Chart | Key Question Answered |
|---|-------|-----------------------|
| 1 | National unemployment trend line | How did unemployment change over time? |
| 2 | Urban vs Rural comparison | Which area was hit harder by COVID? |
| 3 | Top 10 worst-hit states (bar chart) | Which states suffered most? |
| 4 | State × Month heatmap | Where and when was unemployment highest? |
| 5 | Seasonal pattern (pre-COVID) | Are there recurring monthly trends? |
| 6 | Pre-COVID vs COVID box plot | How did the distribution shift? |
| 7 | Top 15 states overall (bar chart) | Which states have structural unemployment issues? |

---

##  Key Findings

- **Pre-COVID average** unemployment: **9.23%**
- **COVID-period average** unemployment: **12.96%** (+3.73 percentage points)
- **Peak month:** May 2020 — national average hit **23.2%**
- **Urban areas** were hit significantly harder (+8.7 pp) than rural areas (+3.1 pp)
- **Top 5 worst-hit states** (Apr–Jun 2020): Puducherry (46.1%), Jharkhand (42.4%), Bihar (36.8%), Haryana (33.0%), Tamil Nadu (31.7%)
- Unemployment spiked within **weeks** of the national lockdown announcement (Mar 24, 2020)

---

## Policy Recommendations

1. **Strengthen urban safety nets** — urban informal workers lost jobs fastest and recovered slowest
2. **Scale up MGNREGS** — rural employment guarantee schemes proved effective as a buffer
3. **Target high-risk states** — Bihar, Jharkhand, and Haryana need dedicated job creation programs
4. **Build pandemic-proof gig worker protections** — informal sector had no safety net during lockdown
5. **Off-season employment programs** — seasonal patterns suggest Dec–Jan demand for supplemental work

---

##  How to Run

1. Open [Google Colab](https://colab.research.google.com)
2. Upload `Unemployment_Analysis.ipynb`
3. Run **Step 2** — a file upload button will appear
4. Upload both CSV files when prompted
5. Run all cells (`Runtime → Run all`)

---

##  Sample Output

The notebook produces charts like these:

-  Smooth trend line with pre-COVID vs COVID colour split
-  State-month heatmap showing the lockdown wave
-  Box plots comparing distributions before and during COVID

---

##  Author

**Syed Mustehsan Akhtar Kazmi**  
Data Science Intern  
