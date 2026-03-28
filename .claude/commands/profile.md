Generate a detailed data profile report for the provided dataset.

Steps:
1. Load the data
2. Basic info: row count, column count, memory usage
3. Per-column report:
   - dtype, null count, null %, unique count
   - For numeric: min, max, mean, median, std, skewness, kurtosis
   - For categorical: top 10 value counts, cardinality
   - For datetime: min date, max date, range, gaps
4. Cross-column checks:
   - Highly correlated pairs (>0.9)
   - Potential ID columns (all unique)
   - Constant or near-constant columns
5. Print a concise summary table
