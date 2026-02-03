# Buffalo Summer Temperature Time-Series Analysis (JJA)
Overview

This repository contains an R-based time-series analysis of historical summer temperatures at the Buffalo Niagara International Airport. Using station-level data from the NASA Goddard Institute for Space Studies (GISS), the project examines long-term trends in June–July–August (JJA) mean temperatures to evaluate whether summer conditions have warmed over time.
The analysis was motivated by a simple empirical question: Are summers in Buffalo hotter today than in the early 20th century? The project demonstrates how publicly available climate data can be transformed into reproducible evidence using modern data science workflows.

# Data
Source: NASA GISS Surface Temperature Analysis (GISTEMP v4)
Station: Buffalo Niagara Airport (USW00014733)
Temporal coverage: Early 1900s to present
Variables used: Annual mean summer temperature (JJA)
Data were accessed directly from the NASA GISS website as a remotely hosted CSV file and imported into R for analysis.

# Methods
The analysis was conducted entirely in R using the tidyverse ecosystem and follows a reproducible, script-based workflow:

 # Data ingestion
1. Downloaded station data directly from NASA GISS using a URL-based import.
2. Handled missing values and standardized column names.

# Data cleaning and preparation
1. Converted year values to numeric format for time-series analysis.
2. Filtered incomplete observations to ensure consistent visualization.

# Time-series visualization
1. Plotted annual JJA mean temperatures to show interannual variability.
2. Added a LOESS-smoothed trend line to highlight long-term patterns.
3. Included clear axis labels, units, and source annotations.

# Exploratory trend analysis
1. Aggregated temperatures by decade to reduce noise and examine broader climate shifts.
2. Compared early- and late-period summer temperature patterns visually.

# Key Findings
Summer temperatures in Buffalo show substantial year-to-year variability, which explains why individual years in the past can feel comparable to recent summers.
Despite this variability, the smoothed time-series trend indicates a long-term increase in mean summer temperatures.
Decadal averages reinforce this pattern, suggesting that recent decades are warmer on average than those in the early 20th century.
These results support the conclusion that while short-term memory can be misleading, long-term climate records provide clear evidence of warming.
