# Cafe Sales Data Analysis Project

## Dataset
- File name: `dirty_cafe_sales.csv`
- Description: Sales data with some missing, invalid, or inconsistent values.

## Project Goals
1. Load and explore the dataset using Python and PyCharm IDE.
2. Clean the data: remove duplicates, correct missing or invalid entries, standardize columns.
3. Ensure logical consistency, especially for calculated fields like `Total_Spent`.
4. Prepare the data for analysis by filling missing values and detecting outliers.
5. Perform exploratory data analysis (EDA) to calculate key sales metrics such as total revenue, average transaction value, popular products, seasonal trends, and daily sales patterns.
6. Visualize the data using Pandas built-in plotting methods: boxplots, line plots, pie charts, and heatmaps to explore sales distributions and co-purchase patterns.
7. Optimize data processing using vectorized operations to improve performance and avoid unnecessary loops or repetitive processing.

## Tools & Libraries
- Python (Pandas, NumPy)
- PyCharm IDE
- Jupyter Notebook (optional)
- Matplotlib / Pandas plotting methods

## Notes
- Data cleaning handles "UNKNOWN" and "ERROR" as missing values.
- Logical consistency checks verify that `Total_Spent` roughly equals `Quantity * Price_Per_Unit` within a tolerance.
- Outliers are detected based on the interquartile range (IQR) method for `Quantity`.
- Vectorized methods (`.str`, `.map`, `.where`) are preferred over `.apply()` for better performance.
- For visualization, simple plots like line, boxplot, and pie chart are created using Pandas `.plot()` method.
- Project includes code examples for filtering, aggregation, and handling missing data.

## How to Use
1. Load the dataset:
   ```python
   import pandas as pd
   df = pd.read_csv('dirty_cafe_sales.csv')
2. Follow steps for cleaning and preparation.

3. Perform analysis and visualization as needed.

4. Update and rerun the notebook or script to keep results up-to-date.

Feel free to modify and extend this project for deeper insights or additional features.
