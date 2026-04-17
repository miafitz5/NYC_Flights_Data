
# NYC Flights Data Analysis

This project explores and visualizes flight data from New York City using the `nycflights13` dataset in R. The analysis is performed in [NYC_Flights_Data.Rmd](NYC_Flights_Data.Rmd), with an HTML report output for easy viewing.

## Overview

The goal is to summarize, join, and visualize flight routes from NYC airports, focusing on data wrangling and mapping techniques in R.

## Steps and Methods

1. **Summarize Origin/Destination Pairs**
	- Counted all unique flight routes (origin/destination pairs) and displayed the first six in a table.

2. **Join Airport Coordinates**
	- Used `left_join` to add latitude and longitude for origin airports, then for destination airports, creating a complete set of coordinates for each route.

3. **Tabular Summaries**
	- Displayed the first six rows after each join to verify the data structure and correctness.

4. **Mapping the USA**
	- Plotted a blank map of the United States using `ggplot2` and `maps` as a base for visualizing flight paths.

5. **Visualizing Flight Frequencies**
	- Drew lines (using `geom_segment`) from origin to destination for each route, with line transparency indicating the number of flights. This highlights the busiest routes from NYC.

6. **Filtering for Continental US**
	- Filtered out flights with destinations outside the continental US to improve map clarity.

## How to Reproduce

1. Open [NYC_Flights_Data.Rmd](NYC_Flights_Data.Rmd) in RStudio or another R Markdown editor.
2. Knit the document to generate the HTML report.
3. All code is chunked and annotated for clarity.

## Requirements

- R (tested with version 4.x)
- Packages: `tidyverse`, `nycflights13`, `dplyr`, `maps`, `ggplot2`, `knitr`

## Output

- [NYC_Flights_Data.html](NYC_Flights_Data.html): The rendered HTML report with all tables, code, and visualizations.

## Author

Mia Fitzgerald
April 16, 2026