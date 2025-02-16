# Virulence Factor Visualization Script

## Description
This script was created to generate a graph based on the results of the VFanalyzer, a tool from the VFDB (The Virulence Factor Database). 
The graph visualizes the number of virulence factors identified in different bacterial strains.

## Features
- Reads input data from a CSV file.
- Filters virulence factors with presence indicated by a value of `1`.
- Generates a horizontal bar plot with custom colors for each virulence factor.

## Prerequisites
To run this script, you need the following:
- R/RStudio installed on your system.
- The following R packages:
  - `ggplot2`
  - `dplyr`
  - `reshape2`

## You can install the necessary packages by running:

install.packages("ggplot2")
install.packages("dplyr")
install.packages("reshape2")

## The script expects a CSV file named latest_spreadsheet.csv structured as follows:

The first row contains column names.
The first column contains strain names.

# Example: ((where 0 indicates absence and 1 indicates presence))

,Strain1,Strain2,Strain3
Factor1,1,0,1
Factor2,0,1,1
Factor3,1,1,0

## How to Run: 
1. Place the last_spreadsheet.csv file in the same directory as the script.
2. Open the script in R or RStudio.
3. Import your latest_spreadsheet.csv

## Output
The script will generate a horizontal bar plot visualizing the number of virulence factors for each strain.
