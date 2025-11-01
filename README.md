
# Ad Traffic IVT Analysis

This project analyzes ad traffic data from multiple apps to understand patterns that lead to Invalid Traffic (IVT) detection.

## Project Overview
We analyzed data from six apps — three valid and three invalid — to understand why some were flagged for IVT.  
Metrics such as **idfa_ip_ratio**, **idfa_ua_ratio**, and **requests_per_idfa** were studied across daily, hourly, and total levels.

## Tools Used
- Python (Pandas, NumPy, Matplotlib)
- Power BI
- Excel

## Key Insights
- Two valid apps showed a sudden spike in **idfa_ua_ratio**, suggesting possible spoofed device behavior.
- Apps marked IVT earlier had consistently abnormal ratios compared to others.
- Stable idfa_ip_ratio indicated that traffic was not geographically diverse.

## Files
- `master_daily.csv`, `master_hourly.csv`, `master_total.csv` → Cleaned data files
- `IVT_Analysis.ipynb` → Python analysis notebook
- `IVT_PowerBI.pbix` → Power BI dashboard

## Summary
The analysis helped identify patterns that indicate when and why certain apps were flagged for IVT. It demonstrates how data analysis can detect suspicious traffic using ratios and time-based patterns.
