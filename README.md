# Credit Risk Bucketing & Expected Loss — FICO-Based Ratings, KMeans Segmentation, PD→EL Mapping

## Overview
Segments borrowers into risk buckets using FICO-based rules and KMeans clustering, visualizes distributions, and connects PD estimates to Expected Loss (EL = PD × LGD × EAD).

## Data
- Uses columns like `fico_score`, `default` (0/1). 
- Ensure the dataset is available locally; do not commit private data.

## Methods
- Rule-based ratings (e.g., 1=best to 5=worst)
- KMeans segmentation for alternative bucketing
- Histograms of FICO by rating
- Expected Loss illustration with configurable LGD/EAD assumptions

## Results
- Ratings distribution (1–5), sample tables
- Visual FICO distribution per rating
- Example EL calculations from PD

## Notes & Limitations
- Ratings here are illustrative; calibrate cut-offs and number of clusters to business data.
- LGD/EAD set as assumptions; replace with empirical estimates where possible.

## What can make this better...
- Calibrate cut-offs using KS/IV or monotonic binning
- Integrate model PDs from `Task_3.ipynb`
- Produce bucket-level PD/LGD/EAD tables for reporting
