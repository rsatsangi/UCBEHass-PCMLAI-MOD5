## 🧠 Project Overview

This project analyzes promotional coupon acceptance behavior using a dataset of coupon offers and associated user interactions. The primary goal is to understand patterns in acceptance rates across different segments such as:

- Time of day
- Age and age groups
- Bar and coffee house coupon responses

The analysis includes statistical summaries and visualization of acceptance rates to derive actionable insights.

---

## 📁 Repository Structure
```bash
UCBEHass-PCMLAI-MOD5/
│
├── data/                          
│   └── coupons.csv              # Raw and processed coupon data
├── Coupons-Data-Analysis.ipynb  # Main Jupyter notebook
│
└── README.md                    # Project documentation
```
---

## 📊 Key Analyses

### 1. Acceptance Rate by Time of Day

Compute and visualize acceptance rates for coupon offers by time slots. The analysis includes:

- Grouping by time of day
- Calculating acceptance rate percentages
- Sorting for highest to lowest performance
- Visualizing results with bar charts

### 2. Age and Demographics

The project explores how age and age buckets affect acceptance behavior by:

- Converting ages from string to numeric
- Creating meaningful age groups (e.g., 21–25, 26–30, etc.)
- Examining acceptance and visit patterns across age segments

### 3. Behavior Patterns

Additional analyses examine:

- How habits (e.g., bar visits frequency) influence coupon acceptance
- Profile differences (e.g., traveling companions)
- Correlation of lifestyle attributes with acceptance

---

## 📈 Visualizations

The notebook includes professional-style visualizations with:

- Grouped bar plots for acceptance vs. rejection
- Label annotations (percentages and labels)
- Reference lines for average acceptance benchmarks
- Custom styling for clarity and presentation quality

---

## 🔧 Dependencies

This project uses Python (≥3.7) with the following libraries:

- `pandas` — data manipulation
- `matplotlib` — visualizations
- `seaborn` — statistical plots
- `numpy` — numeric operations
- Jupyter Notebook (`.ipynb`) for interactive analysis
