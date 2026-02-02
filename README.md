# Module 1: Tabular Data

## Overview

This module explores high-performance workflows for tabular data using `duckdbfs` to work with datasets that are larger than available RAM by leveraging DuckDB's streaming and remote file access capabilities.

## Case Study: Global Supply Chains

We work with [EXIOBASE 3.8.1](https://source.coop/youssef-harby/exiobase-3), a global Multi-Regional Input-Output (MRIO) database that tracks economic transactions between sectors and regions, along with their environmental impacts (emissions, resource use, etc.).

### Data Description
- **Coverage**: 44 countries + 5 rest-of-world regions
- **Timeframe**: 1995–2022
- **Content**: Economic transactions (Z matrix), final demand (Y matrix), and environmental stressors (F matrix)
- **Format**: Cloud-optimized Parquet, partitioned by year and matrix type

## Getting Started

The main analysis is in `tabular-data.qmd`, which includes:
- Exercise 1: Connecting to remote data
- Exercise 2: Efficient filtering and querying

### Requirements
- R
- `duckdbfs` package
- `dplyr` package

## Course
ESPM 288
