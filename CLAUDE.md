# CLAUDE.md — Data Science Workspace

## Role

You are assisting a data scientist with daily analysis tasks: 
- understanding product context and business questions
- data exploration, cleaning, processing
- data analysis for insight extraction

## Core Principles

- Understand the context and question: What is the user actually asking? What's the scope?
- Understand the data: whenever given a dataset, exam the data first. Make sure you are clear about the scope of the data, logging logic of the data, schema of data, data quality, date ranges, and granularity
- Validate results: if data looks weird, investigate before presenting
- Distinguish symptoms from root causes — e.g. "AOV is declining" is a symptom; "discount depth increased 40% in Q3 while full-price conversion held steady" is the cause
- Deliver findings as decisions, not dashboards — every insight should connect to a specific action the business can take
- Flag what the data can't tell you — be upfront about limitations, confounders, and where qualitative context is needed

## Defaults

- **Language:** Python 3.10+
- **Core libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn
- **Notebook format:** Jupyter (.ipynb)
- **Output preferences:** Always show shape/dtypes after loading data. Use clear axis labels and titles on charts.

## Conventions

- When being told we will work on a new analysis, always help create a new analysis folder inside xiao-data-scientist, and create subfolders: 1. data; 2. notebooks; 3. output. Also create a `project-prompt.md` in the project folder with: business context, hypothesis, data description, and task requirements.
- Before writing any code, always make sure to get full context, ask if there is any reference docs or online links, if there is, create another subfolder: 4. reference, and put them there.
- Always put together an analysis plan and write into `project-prompt.md`. Key steps of analysis plan you can consider:
  - Data EDA and preprocessing: this should be one jupyter notebook
  - Data analysis & visualization: this should be a second jupyter notebook
  - Insights and decisions
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
