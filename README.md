# Bootstrap Analysis Project

## Overview
This project involves analyzing voting support rates using a bootstrap simulation technique. The data is collected from a sample of likely voters in the United States, 
and the goal is to estimate the average support rates for the Republican and Democrat parties. We use a resampling method with replacement to approximate the variability 
in the original dataset and compute average support rates.
![image](https://github.com/user-attachments/assets/6718a15d-740d-4904-97af-dd3c0a65c82b)
## Files Included
- **us_voters_with_votes_sample_data.csv**: The dataset containing voter demographic information and their respective votes. The dataset is randomly generated from
  `Atlas National Poll - United States Presidential Election 2024` with data from `10/25/2024 - 10/29/2024`.
- **bootstrap_analysis.ipynb**: The script that performs the bootstrap simulation, calculates the average support rates for the Republican and Democrat parties, and
visualizes the results.

## Methodology
- **Data Preparation**: The dataset contains information about voting preferences and demographics. Voters are categorized by their party support (Republican, Democrat,
Other, etc.), and the script maps each candidate to their respective party using a dictionary.

- **Bootstrap Simulation**: The bootstrap method is used to create new samples from the original data by resampling with replacement. Each iteration of the bootstrap
 produces a sample from which party support rates are calculated. We repeat this process 1000 times to get a distribution of support rates.

- **Calculations and Visualization**: After the bootstrap iterations, the average support rates for the Republican and Democrat parties are calculated. We also use a
 simple moving average (SMA) with a window size of 5 to smooth out the results, which are then visualized in a line plot.


