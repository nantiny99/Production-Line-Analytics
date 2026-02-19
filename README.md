# Production-Line-Analytics

## Overview
This project analyzes a production line dataset to identify efficiency, downtime causes, and operator performance. Using real batch production data, the analysis provides insights for improving productivity and reducing operational errors.

## Data
The analysis uses four datasets:

- **`line-productivity.csv`** – Batch-level production data with start/end times and operator information.
- **`products.csv`** – Product details including flavor, size, and minimum batch time.
- **`line-downtime.csv`** – Downtime minutes for each batch, broken down by factor.
- **`downtime-factors.csv`** – Downtime factor descriptions and whether they are operator errors.

## Questions Addressed

### Existing Line Efficiency
- Calculated as **Minimum Batch Time / Actual Batch Time**.
- Shows overall production efficiency and highlights operators performing below expectations.

### Operator Performance
- Identifies operators whose average batch efficiency falls below line standards.
- Highlights patterns for targeted training or process improvements.

### Primary Causes of Downtime
- Aggregates total downtime by factor.
- Visualized using horizontal bar charts and Pareto charts to identify the largest contributors to lost production time.

### Operator Challenges with Errors
- Analyzes downtime due to operator errors per operator and per error type.
- Visualized using a heatmap to identify specific areas for improvement.

## Tools & Techniques
- **Python** with `pandas` for data manipulation.
- **Matplotlib / Seaborn** for visualization.
- Aggregation, merging, and pivoting of fact and dimension tables.
- Root-cause analysis and Pareto charts for identifying major contributors.

## Insights
- A few key downtime factors contribute the majority of lost production time.
- Certain operators have recurring errors associated with specific downtime factors.
- Targeted interventions on both process and training can improve overall efficiency.
