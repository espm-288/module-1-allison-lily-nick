# Module 1: Tabular Data

**Team Members:** Allison, Lily, Nick  
**Course:** ESPM 288

## Overview

This module explores high-performance workflows for tabular data using `duckdbfs` to work with datasets that are larger than available RAM by leveraging DuckDB's streaming and remote file access capabilities.

## Case Study: Global Supply Chains

We work with [EXIOBASE 3.8.1](https://source.coop/youssef-harby/exiobase-3), a global Multi-Regional Input-Output (MRIO) database that tracks economic transactions between sectors and regions, along with their environmental impacts (emissions, resource use, etc.).

### Data Description
- **Coverage**: 44 countries + 5 rest-of-world regions
- **Timeframe**: 1995–2022
- **Content**: Economic transactions (Z matrix), final demand (Y matrix), and environmental stressors (F matrix)
- **Format**: Cloud-optimized Parquet, partitioned by year and matrix type

## Files

- `tabular-data.qmd` - Main analysis notebook with exercises

## Setup

### Prerequisites

- R (version 4.5+)
- Required packages: `duckdbfs`, `dplyr`

### Installation

```r
install.packages("duckdbfs")
install.packages("dplyr")
```

### Running the Analysis

Open `tabular-data.qmd` in RStudio or another Quarto-compatible editor and run the code chunks.

## Exercises

1. **Connecting to Remote Data** - Access cloud-hosted EXIOBASE data without downloading
2. **Efficient Filtering** - Query large datasets using lazy evaluation
3. **Task** - Find top 5 US sectors by CO2 emissions in 2022
