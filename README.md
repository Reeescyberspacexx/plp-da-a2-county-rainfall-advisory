# County Rainfall and Planting Advisory

**Author:** Marion Oduor · PLP Data Analytics Cohort 2026

## Problem

A farmer-support NGO sends SMS planting advice to farmers in five counties (Nairobi, Nakuru, Kisumu, Mombasa and Machakos). Its monthly rainfall data is mostly clean, but the Machakos record was typed by hand and contains invalid entries. This project cleans that record, analyses the rainfall patterns with NumPy (core Python and NumPy only, no pandas), and recommends a planting window for each county, saved as `rainfall_summary.csv`.

## How to Run

[Open in Colab](https://colab.research.google.com/github/Reeescyberspacexx/plp-da-a2-county-rainfall-advisory/blob/main/rainfall_analysis.ipynb), then select Runtime → Run all. Install the libraries with `pip install -r requirements.txt` if running outside Colab.

## Key Findings

1. **Four counties share one window:** April to May is the wettest two-month period in Nairobi, Nakuru, Kisumu and Mombasa, with Kisumu highest at 420 mm combined.
2. **Machakos is different and driest:** its best window is November to December (278 mm combined), its annual total is only 811 mm, and it has 6 dry months, the most of any county.
3. **Machakos data was repaired:** 2 of its 12 readings (April and September) were invalid and were replaced with the average of 68 mm, so its advice should be confirmed.
