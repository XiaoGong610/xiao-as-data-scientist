Clean and preprocess the provided dataset.

Steps:
1. Load the data and profile it (shape, dtypes, nulls, duplicates)
2. Handle missing values — point out missing value problem, report strategy for each column (drop, impute mean/median/mode, fill forward, etc.)
3. Remove or flag duplicates
4. Fix data types (dates as datetime, categories as category, numerics parsed correctly)
5. Standardize string columns (strip whitespace, consistent casing)
6. Detect and handle outliers (report them, don't remove unless instructed)
7. Save the cleaned dataset as a new file
8. Print a before/after summary (row count, null count, dtype changes)

Document every transformation applied.
