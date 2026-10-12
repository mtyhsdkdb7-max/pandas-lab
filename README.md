# PandasLab — Visual Data Analysis Workbench

A browser-based interactive data analysis workbench inspired by Python's pandas library. No coding required — load your CSV, clean, transform, and visualize data entirely through a GUI.

**Live Demo:** [https://4m87jh6c5pg1k.doubaoapps.com/app/app_17fsyysjw37](https://4m87jh6c5pg1k.doubaoapps.com/app/app_17fsyysjw37)

![Dark theme data analysis interface](screenshot.png)

## Features

### Data Loading
- Built-in default e-commerce sales dataset (240 rows, 13 columns)
- Upload your own CSV files with automatic type detection
- One-click reset to default data

### Data Inspection
| Operation | pandas equivalent |
|-----------|-------------------|
| Head / Tail | `df.head(n)` / `df.tail(n)` |
| Data overview | `df.info()` |
| Statistical summary | `df.describe()` |
| Column types | `df.dtypes` |
| Missing values | `df.isna().sum()` |

### Data Cleaning
- `dropna()` — drop rows/columns with missing values
- `fillna()` — fill with mean, median, mode, or custom value
- `drop_duplicates()`
- `rename()` columns
- `drop()` columns
- `astype()` type conversion

### Data Transformation
- `query()` — conditional filtering (>, <, >=, <=, ==, !=)
- `sort_values()` — sort by any column
- `groupby().agg()` — group + aggregate (mean, sum, count, min, max, median, std)
- `value_counts()` — frequency counts
- Column subset selection

### Visualizations (ECharts)
- **Histogram** — distribution of numeric columns
- **Scatter plot** — correlation between two numeric columns, with optional group coloring
- **Bar chart** — category vs numeric comparison
- **Line chart** — trends over time
- **Box plot** — distribution by category
- **Correlation heatmap** — Pearson r matrix with annotations
- **Pie chart** — category proportions

### Other
- Bilingual UI (Chinese / English toggle)
- Operation history bar
- Paginated data table with sortable headers
- Dark professional theme

## Tech Stack
- Pure HTML/CSS/JS single file, no build step
- [ECharts 5](https://echarts.apache.org/) for charts
- [Papa Parse](https://www.papaparse.com/) for CSV parsing
- [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) + [JetBrains Mono](https://www.jetbrains.com/lp/mono/) fonts

## Usage
1. Open `index.html` in any modern browser, or visit the live demo link above
2. Explore the default dataset, or click **Load CSV** to upload your own
3. Use the left sidebar for data operations
4. Switch to the **Charts** tab for visualization

## Project Structure
```
pandas-lab/
├── index.html      # The entire application (single file)
├── README.md
└── 功能说明.md      # Chinese feature documentation
```

## License
MIT
