# UciCreditDefault

Data analysis on a simulated credit card default dataset.

This repository demonstrates the author's journey and growth in the fields of data analysis and data science. The initial Python program was coursework submitted for a Machine Learning class. It showcased a basic understanding of data preparation and machine learning principles.

The author is now revisiting and enhancing the project while completing the [Google Data Analytics Professional Certificate](https://grow.google/dataanalytics/). This updated version incorporates best practices learned from the course, including improved data cleaning, visualization, and analysis techniques.

## Project Objectives

- Showcase personal growth in data analysis and data science.
- Apply new knowledge from the Google Data Analytics Professional Certificate.
- Provide a comparative view of initial versus updated approaches to data analysis.

## Dataset Attribution

This project uses the UCI Credit Card Default dataset:

- **Direct Source**: [UCI Credit Card Default Dataset](http://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients)
- **License**: [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)
- **Accessed via**: Kaggle

The raw dataset is included in this repository under `data/raw/UCI_Credit_Card_original.csv`. Attribution is required for reuse.

This dataset is distributed under the terms of the [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0/), which permits sharing and adaptation with attribution.

## Current Progress

The project currently includes:
1. **Raw Dataset**:
   - Directly downloaded from the UCI Machine Learning Repository.
2. **Cleaned Dataset**:
   - Includes the latest cleaned version (`v4.3.3`) with:
     - Consolidated ambiguous values in the `EDUCATION` column.
     - Converted numerical columns (`MARRIAGE`, `SEX`) to textual labels.
     - Added a new column `Pay Status Word` for clearer interpretation of `PAY_X` values.

## Key Improvements

- **Ambiguous Values**: Consolidated unknown `EDUCATION` levels into a single category (`Unknown`) for clarity.
- **Column Headers**: Renamed technical headers to user-friendly names (e.g., `PAY_X` → `Pay Status`).
- **Textual Labels**: Converted numerical columns (`SEX`, `MARRIAGE`) to descriptive textual labels for better interpretability.
- **New Column**: Added `Pay Status Word` to provide clear interpretations of payment status.

## Progress and Changelog

Detailed cleaning and transformation steps are documented in [changelog/progress.md](changelog/progress.md).

## Visualizations (Coming Soon)

Interactive and static visualizations showcasing the dataset's structure and key insights will be added to the repository.

## Future Plans and Additions

- Perform exploratory data analysis (EDA) to identify trends and correlations.
- Create dashboards in Tableau for interactive visualization.
- Apply machine learning models to predict credit default risk.
- Include visualizations and insights from the cleaned dataset.
- Showcase the results of an initial machine learning model using the cleaned data.

## Contact

- **Author**: Johnpaul Medina
- **Email**: jmedinacs715@gmail.com
- **GitHub**: [https://github.com/jmedinacs](https://github.com/jmedinacs)
