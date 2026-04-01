# Description 

In this project I aim to apply all the knowledge, skills and abilities developed throughout the Bootcamp. To do so, I have chosen a well-documented topic - the COVID-19 pandemic - focusing on the effectiveness of vaccine administration during that period. The analysis is based on two publicly available datasets sourced from the WHO.

# Objectives 
# Datasets 
# Project Structure 
# Requirements 
# Results/Conclusions

COVID-19 Dataset – Cleaning Summary

This dataset has been processed and cleaned for analysis. Key steps included:

Initial inspection – Explored dataset structure, summary statistics, and data types.
Handling missing values –
Forward filled New_cases and New_deaths per country to address reporting gaps.
Remaining NaNs correspond to the earliest reported dates; cumulative counts on these dates are zero, so these are assumed to represent true zero values.
Duplicates – Checked and removed any duplicate rows.
Column adjustments – Renamed columns for clarity and converted data types as needed.
Timeframe alignment – Adjusted the dataset’s date range to match the intended timeframe for future merges (e.g., with vaccines dataset).

This cleaned version has been exported to data/processed/covid_cleaned.csv and is ready for analysis or further processing. All cleaning decisions are documented to maintain data integrity and reproducibility.