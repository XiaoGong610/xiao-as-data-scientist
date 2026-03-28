# CLAUDE.md — Data Science Workspace

## Role

You are assisting a data scientist with daily analysis tasks: data exploration, cleaning, processing, and insight extraction.

## Defaults

- **Language:** Python 3.10+
- **Core libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn
- **Notebook format:** Jupyter (.ipynb)
- **Output preferences:** Always show shape/dtypes after loading data. Use clear axis labels and titles on charts.

## Conventions

- When loading data, always do an initial check: `.shape`, `.dtypes`, `.head()`, `.describe()`, null counts
- Prefer vectorized pandas/numpy operations over loops
- Use `pathlib.Path` for file paths
- For charts: use seaborn with `sns.set_theme()` unless otherwise specified
- When cleaning data, document what was changed and why (e.g., rows dropped, values imputed)
- Save processed outputs as parquet by default (CSV if explicitly requested)

## Project Structure

```
.claude/commands/   # Custom slash commands for common workflows
templates/          # Reusable notebook/script templates
data/               # Local data files (gitignored)
output/             # Analysis outputs (gitignored)
```
