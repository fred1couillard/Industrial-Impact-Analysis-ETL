# Industrial Production & Environmental Impact Analysis

## Objective
As part of a Data Analytics workflow simulation, the goal was to audit the correlation between production spikes (pre-holiday rush) and environmental degradation (PM2.5 levels).

## The Challenge
I worked with raw, unstructured logs containing simulated real-world errors:
* **Inconsistent Naming Conventions:** (`Usine_A` vs `usine a`) requiring string normalization.
* **Date Format Mismatch:** Merging disparate time-series formats (`DD-MM-YYYY` vs `YYYY/MM/DD`).
* **Data Quality:** Handling missing values (NaN) and noisy input types (strings in integer columns).

## Methodology
1.  **Data Cleaning (Pandas):** Implemented a cleaning pipeline to standardize factory names and convert types.
2.  **Data Merging:** Performed an `Inner Join` to align production logs with sensor data.
3.  **Statistical Inference:** Calculated Pearson correlation coefficient (**0.86**) to validate the hypothesis.

## Key Finding
The analysis revealed a **strong positive correlation (0.86)**, confirming that production surges in December are the direct driver of local air quality drops.

## Tech Stack
* Python, Pandas (Data Manipulation)
* Matplotlib, Seaborn (Visualization & Trend Analysis)
