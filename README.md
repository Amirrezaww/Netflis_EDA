# Netflix EDA (Exploratory Data Analysis)

This repository contains an exploratory data analysis (EDA) project analyzing Netflix titles data using Jupyter Notebooks.

## Overview

The `test2.ipynb` notebook performs comprehensive exploratory data analysis on Netflix's catalog of movies and TV shows. The analysis includes data cleaning, visualization, and insights about content trends, particularly focusing on the differences between Movies and TV Shows added to the platform over time.

## Features

### Data Analysis
- **Content Type Comparison**: Analyzes and compares Movies vs TV Shows in the Netflix catalog
- **Temporal Analysis**: Examines trends in titles added to Netflix over time
- **Time Series Visualization**: Creates visualizations showing monthly additions of content
- **Data Smoothing**: Uses rolling averages to identify trends and patterns

### Key Visualizations
- **Monthly Additions Chart**: Line plot showing the number of titles added per month, with separate trends for Movies and TV Shows
- **3-Month Rolling Average**: Smoothed visualization to highlight long-term trends and reduce daily noise

## Key Insights

Based on the analysis:

- **Content Cycles**: Movies are added in larger, more volatile batches, while TV Shows follow steadier patterns
- **Peak Addition Period**: Movies reached peak additions in late 2019 (~180 titles per month)
- **Impact Events**: Notable drop in Movie additions during 2020, likely due to COVID-19 pandemic impacts
- **Platform Evolution**: Analysis reveals the evolution of Netflix's content strategy over time

## Requirements

To run this notebook, you'll need:

- Python 3.x
- Jupyter Notebook or JupyterLab
- Required Python libraries:
  - `pandas` - For data manipulation and analysis
  - `numpy` - For numerical operations
  - `matplotlib` - For data visualization

## Installation

1. Clone this repository or download the files
2. Install required dependencies:

```bash
pip install pandas numpy matplotlib jupyter
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `test2.ipynb` in the Jupyter interface

## Usage

1. Ensure you have the Netflix dataset (the notebook expects a DataFrame named `df` with the following columns):
   - `date_added`: Date when title was added to Netflix
   - `type`: Content type (Movie or TV Show)
   - Other relevant columns for Netflix titles analysis

2. Run all cells in the notebook to execute the analysis

3. Review the visualizations and insights generated

## Data Structure

The notebook expects a pandas DataFrame with at least the following columns:
- `date_added`: Datetime column indicating when titles were added
- `type`: String column with values "Movie" or "TV Show"

## Notebook Structure

- **Data Preprocessing**: Handles datetime conversion and data cleaning
- **Data Analysis**: Groups and resamples data by month
- **Visualization**: Creates time series plots with smoothing
- **Insights**: Provides key takeaways from the analysis

## Notes

- The notebook handles missing data using pandas operations
- Date parsing uses flexible format handling to accommodate various date formats
- Visualizations are optimized for readability with proper labeling and legends

## License

See the LICENSE file for details.

## Author

Created as part of exploratory data analysis learning and practice.
