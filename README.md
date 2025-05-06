# World Population Analysis 2024

This repository contains a Python script for analyzing world population data for the year 2024. The script performs data cleaning, exploratory data analysis (EDA), and generates visualizations to understand population trends, area distribution, and population change across different countries.

## Data Source

The data is sourced from a CSV file hosted on GitHub:

[Dataset Link](https://raw.githubusercontent.com/manya-gangoli/World-Population-2024-EDA-and-prediction/refs/heads/main/World%20Population%20by%20country%202024.csv)

## Libraries Used

The following Python libraries are used in this analysis:

-   **pandas:** For data manipulation and analysis.
-   **numpy:** For numerical operations.
-   **matplotlib.pyplot:** For creating static, interactive, and animated visualizations in Python.
-   **seaborn:** For making statistical graphics in Python.
-   **warnings:** To handle and filter warning messages.

## Data Cleaning

The data cleaning process involves the following steps:

-   Loading the CSV file into a pandas DataFrame.
-   Calculating the 'Population Change' by subtracting the 'Population 2023' from the 'Population 2024'.
-   Converting the 'Area (km2)' column to a numeric format by handling values with 'M' (millions) and 'K' (thousands) suffixes, as well as values starting with '<'. The column is then cast to a float data type.

## Data Analysis and Visualization

The analysis includes visualizing the following:

-   **Top 10 Countries with Highest Population:** A bar plot showing the countries with the largest populations in 2024.
-   **Last 10 Countries with Least Population:** A bar plot displaying the countries with the smallest populations in 2024. The x-axis is inverted for better readability.
-   **Top 10 Countries with Highest Area:** A bar plot illustrating the countries with the largest land areas.
-   **Last 10 Countries with Lowest Area:** A bar plot showing the countries with the smallest land areas. The x-axis is inverted.
-   **Top 10 Countries with Highest Population Change:** A bar plot highlighting the countries with the largest increase in population from 2023 to 2024.
-   **Countries with Negative Growth Rate:** A scatter plot showing countries with a negative population growth rate.
-   **Density vs Area:** A scatter plot visualizing the relationship between a country's area and its population density, with the color of the points indicating the growth rate.

## Observations

The analysis yielded the following key observations:

1.  **India** has the highest population in 2024.
2.  **Vatican City** has the lowest population in 2024.
3.  **Russia** has the largest land area.
4.  **Vatican City** has the smallest land area.
5.  **India** experienced the highest population increase from 2023 to 2024.
6.  There are **42 countries** with a negative population growth rate, including China and Russia.
7.  **Moldova** has the most significant negative population growth rate.
8.  Countries with small land areas often have very high population densities, with some exceptions like Russia and China, which have large areas but relatively lower densities.

## How to Use

1.  Clone this repository to your local machine.
2.  Ensure you have the required libraries installed (`pandas`, `numpy`, `matplotlib`, `seaborn`). You can install them using pip:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
3.  Run the Python script (the provided code snippet) to perform the analysis and generate the visualizations. The plots will be displayed on your screen.
