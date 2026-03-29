# xiao-as-data-scientist

Claude Code setup for data science workflows.

## Setup

1. Clone this repo
2. Open it in Claude Code: `cd xiao-as-data-scientist && claude`

## Custom Commands

| Command | Description |
|---------|-------------|
| `/data-eda` | Exploratory data analysis: profile columns, check correlations, plot distributions |
| `/data-preprocessing` | Clean and preprocess a dataset: handle missing values, duplicates, types, outliers |
| `/analysis-experiment` | Analyze A/B experiments: compare metrics, check randomization balance |
| `/analysis-funnel` | Analyze funnel conversion: stage rates, drop-off visualization, segmentation |
| `/summary-slides` | Generate a PowerPoint summary of analysis findings via python-pptx |

## Structure

```
CLAUDE.md               # Instructions for Claude Code
.claude/commands/       # Custom slash commands
templates/              # Reusable templates
data/                   # Local data files (gitignored)
output/                 # Analysis outputs (gitignored)
```
