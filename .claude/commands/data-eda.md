Perform exploratory data analysis on the provided dataset.

Steps:
1. Load the data and display shape, dtypes, and first few rows
2. Data profiling:
   - Per-column report: dtype, null count, null %, unique count
   - For numeric: min, max, mean, median, std, skewness, kurtosis
   - For categorical: top 10 value counts, cardinality
   - For datetime: min date, max date, range, gaps
3. Check for missing values and duplicates
4. Cross-column checks:
   - Highly correlated pairs (>0.9)
   - Potential ID columns (all unique)
   - Constant or near-constant columns
5. Plot distributions of numeric columns (histograms)
6. Plot counts of categorical columns (bar charts)
7. Show a correlation heatmap for numeric features
8. Summarize key findings and potential data quality issues
9. Give recommendation if data pre-processing is needed or not

Use pandas and seaborn. Write the analysis in a Jupyter notebook.
