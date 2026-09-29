# Kansas City, Missouri 2024 Crime Data Analysis

A descriptive analysis of Kansas City Police Department (KCPD) reported crime data for 2024. The project cleans and explores the dataset, then uses interactive geospatial visualizations to inspect where records with usable coordinates appear across the city.

## Explore the analysis

- [Open the interactive geospatial analysis (HTML)](kansas-city-crime-geospatial-analysis.html)
- [View the HTML in NBViewer](https://nbviewer.org/github/AnalyzerArik/Kansas-City-Missouri-2024-Crime-Data-Analysis-/blob/main/kansas-city-crime-geospatial-analysis.html)

The HTML preserves the interactive maps and charts, including area-level incident markers, heatmaps, and views by domestic-violence flag, gender, and offense description.

## Data and scope

- **Source:** [KCPD Crime Data 2024](https://data.kcmo.org/Crime/KCPD-Crime-Data-2024/isbe-v4d8/about_data)
- **Snapshot analyzed:** 95,932 rows and 24 columns in the notebook export included here.
- **Geographic scope:** Kansas City, Missouri, as reported by KCPD; this is not Kansas City, Kansas data.
- **Fields used or explored:** report and occurrence dates, offense description, patrol area, reporting district, domestic-violence flag, involvement, demographic fields, firearm-used flag, and location.

This README describes the repository's saved analysis and snapshot. The source dataset may be updated after that snapshot.

## What the analysis shows

These are descriptive counts from the notebook outputs, not population-adjusted rates.

- **Reported volume differs by patrol area.** Among the 93,795 records with usable coordinates, the map's area counts are CPD **27,471**, EPD **21,862**, MPD **18,554**, SPD **9,419**, NPD **8,747**, SCP **7,396**, OSPD **343**, and UNSPECIFIED **3**. CPD has the largest mapped count in this snapshot. These totals describe recorded volume; they do not show that residents or visitors in one area face a higher individual risk.
- **Five offense descriptions account for 48,260 records with a nonmissing description.** The notebook's top-five chart lists Simple Assault (**12,173**), Motor Vehicle Theft (**10,977**), Vandalism/Destruction of Property (**9,780**), Aggravated Assault (**9,267**), and Shoplifting (**6,063**). The dataset has 87,350 nonmissing Description values, so the five categories represent about **55%** of records with a description.
- **7,617 rows are flagged as domestic violence.** That is about **7.9%** of the 95,932 rows; 88,315 are not flagged. The notebook includes a domestic-violence heatmap for geographic exploration, but it does not quantify a statistically tested spatial cluster.
- **Location coverage is high but incomplete.** The notebook reports coordinates for 93,795 of 95,932 rows; **2,137** lack a usable location and are not represented in coordinate-based maps.

## Why this matters for analyst and BI work

The project demonstrates a useful reporting workflow: inspect field completeness, prepare coordinates, summarize counts by category and area, and make results explorable in charts and maps. For an analyst or BI role, the main practical lesson is to make the measure and its denominator visible. A raw-count map can help teams decide where to investigate service demand or reporting patterns, while a fair comparison of risk across areas would require appropriate population or exposure denominators and clearly defined geographic boundaries.

The category counts also suggest a dashboard design: lead with the most frequent offense descriptions, then let users filter by time, area, and available incident attributes. Data-quality indicators should sit alongside the visuals so users can see when missing descriptions, locations, or reporting districts limit a particular view.

## Limitations and interpretation

- **Counts are not rates.** The notebook does not adjust area totals for resident population, visitors, land area, or other exposure. It cannot support claims that one district or neighborhood is more dangerous.
- **The analysis is descriptive.** Heatmaps visualize the locations included in the file; no statistical spatial-cluster test or causal analysis is documented. The maps should be read as exploratory views.
- **Some fields are incomplete.** The notebook reports 8,582 missing Description values, 9,881 missing reporting districts, 12,208 missing Race values, 11,160 missing Sex values, 26,281 missing Age values, and 2,137 missing locations. Patterns using these fields may reflect incomplete reporting as well as the underlying records.
- **The firearm field is present, but no firearm rate or offense breakdown is reported in the artifact.** This README makes no claim about firearm involvement.
- **This is a saved 2024 dataset snapshot.** It does not establish current conditions or changes over time.

## Tools

Python, Jupyter Notebook, pandas, NumPy, Folium, Plotly, Matplotlib, and Seaborn.
