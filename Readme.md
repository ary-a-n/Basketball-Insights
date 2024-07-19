# Basketball-Insights

## Project Overview

This project involves an in-depth analysis of NBA performance data, including both historical and recent statistics. The objective is to explore and visualize trends, uncover insights, and evaluate the impact of various performance metrics on team success. The analysis spans multiple parts, including data collection, cleaning, and exploration.

## Project Components

### Part I: Data Collection - NBA Web Scraping

1. **Set Up Environment:**
   - Install necessary packages: `pandas`, `requests`, `beautifulsoup4`, `numpy`, `matplotlib`, `seaborn`.

2. **Web Scraping:**
   - Identify URLs for relevant data tables on the Basketball Reference website.
   - Use `requests` to retrieve HTML content.
   - Parse HTML with `BeautifulSoup` to extract data tables.
   - Store the extracted data in `pandas` DataFrames.

3. **Save Data:**
   - Save the scraped data as CSV files for future use.

### Part II: Data Cleaning - NBA Data Cleaning

1. **Load Data:**
   - Load the scraped data from CSV files into `pandas` DataFrames.

2. **Initial Cleaning:**
   - Remove duplicate rows and handle missing values.
   - Drop unnecessary columns.

3. **Data Type Conversion:**
   - Convert columns to appropriate data types (e.g., integers, floats, datetime).

4. **Create Finals Ranking Column:**
   - Manually create a column named `Finals_Ranking` with values: Champion, Runner-Up, Knocked Out, Never Qualified.

5. **Merge Datasets:**
   - Merge multiple datasets into a single DataFrame if applicable.

6. **Save Cleaned Data:**
   - Save the cleaned and merged data as a new CSV file.

## Data Files

- **total_stats_df.csv:** Raw dataset of total stats from 1980-2024 from Basketball Reference.
- **avg_stats_df.csv:** Raw dataset of average stats from 1980-2024 from Basketball Reference.
- **advanced_stats_df.csv:** Raw dataset with advanced metrics (e.g., Margin of Victory, Offensive Rating, Defensive Rating) from 1980-2024.
- **season_summary_df.csv:** Raw dataset with seasonal summaries (e.g., Champions, Runner-up) from 1980-2024.
- **cleaned_total_stats.csv:** Cleaned dataset with total stats and Finals rankings (Finals_Rk).
- **cleaned_avg_stats.csv:** Cleaned dataset with average stats, Finals rankings (Finals_Rk), Age, and Wins.
