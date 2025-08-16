# Online Advertising Performance Analysis

This repository contains a complete analytics workflow for evaluating online advertising performance
from April 1, 2020 to June 30, 2020. It includes a **synthetic sample dataset**, a **Jupyter Notebook**
with detailed analysis & visualizations, and ready-to-use **KPIs**.

## Data Columns
- **Day**: Date of the campaign
- **Campaign**: Campaign segment name
- **User Engagement**: Targeted user behavior (e.g., High/Medium/Low Intent)
- **Banner**: Ad size (e.g., 300x250, 728x90, 160x600, 320x50)
- **Placement**: Publisher space (Website/App category)
- **Displays**: Number of ad impressions served
- **Cost**: Media cost (USD)
- **Clicks**: Number of clicks
- **Revenue**: Click revenue (USD)
- **Post Click Conversions**: Conversions within 30 days after click
- **Post Click Sales Amount**: Sales amount within 30 days after click

## Derived Metrics
- **CPC** = Cost / Clicks
- **RPC** = Revenue / Clicks
- **CR**  = Post Click Conversions / Clicks
- **AOV** = Post Click Sales Amount / Post Click Conversions
- **ROI** = (Revenue − Cost) / Cost

## How to Run
1. Open the notebook at `notebooks/ads_performance_analysis.ipynb`.
2. Run all cells to reproduce the analysis on the provided sample dataset at `data/online_ads_sample.csv`.
3. To use your own data, replace the `DATA_PATH` in the notebook with your CSV/Excel path
   (ensure the same column names).

## Visualizations
Built with **matplotlib** only (one figure per chart, no custom colors).

## Project Structure
```
online_ads_project/
├─ data/
│  └─ online_ads_sample.csv
├─ notebooks/
│  └─ ads_performance_analysis.ipynb
├─ reports/
└─ README.md
```

## Notes
- The included sample data is synthetically generated for demonstration and testing.
- Replace it with your real dataset to obtain production insights.
