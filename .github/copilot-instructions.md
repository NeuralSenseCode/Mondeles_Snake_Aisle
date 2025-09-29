# AI Agent Instructions for Mondeles Snake Aisle

## Project Overview
This is a data science project scaffold for client "Mondeles Snake Aisle" under NeuralSense. The project follows a structured data science workflow with clear separation between exploratory work, production analysis, and results.

## Directory Structure & Purpose

### Core Workflow
- **`data/`** - Raw datasets (gitignored except `.gitkeep`). Never commit PII or confidential data
- **`notebooks/`** - Exploratory data analysis (EDA). Keep outputs stripped when committing
- **`src/`** - Reusable Python modules for processing, models, and utilities
- **`analysis/`** - Production-grade analysis scripts and polished notebooks for reporting
- **`results/`** - Generated outputs (figures, tables, exports). Treat as build artifacts

### Development Environment
- Python-based with core data science stack: pandas, numpy, matplotlib, seaborn, jupyter
- Install dependencies: `pip install -r requirements.txt`
- VS Code workspace configured to exclude `data/` from analysis and hide `__pycache__`

## Key Development Patterns

### Data Handling
- Place sample/test data in `data/` but never commit actual client data
- Reference data files using relative paths from project root: `data/filename.csv`
- Create data loading utilities in `src/` for consistent data access patterns

### Code Organization
- **Exploration phase**: Start in `notebooks/` for initial analysis and visualization
- **Productionization**: Extract reusable functions to `src/` modules
- **Reporting**: Create polished analysis in `analysis/` directory
- Import from `src/` using: `from src.module_name import function_name`

### Notebook Conventions
- Keep exploratory notebooks in `notebooks/` with descriptive names
- Strip cell outputs before committing (mentioned in `notebooks/README.md`)
- Move finalized analysis notebooks to `analysis/` for client delivery

## Client Project Context
- This is scaffolding for "Mondeles Snake Aisle" - adapt code and analysis to retail/consumer context
- Maintain professional standards suitable for client delivery
- Results in `results/` directory should be client-ready outputs

## Quick Start for New Features
1. Create exploration notebook in `notebooks/` for initial data analysis
2. Extract reusable functions to appropriate module in `src/`
3. Create production analysis script/notebook in `analysis/`
4. Save final outputs (charts, tables, reports) to `results/`

## Dependencies & Environment
- Standard data science stack already configured in `requirements.txt`
- Add new dependencies to `requirements.txt` when needed
- Python analysis excludes `data/` directory (see workspace settings)