# UciCreditDefault

**Data Analysis on a Simulated Credit Card Default Dataset**

This repository documents the author's journey and growth in the fields of data analysis and data science. It began as a coursework project for a Machine Learning class, demonstrating an initial understanding of data preparation and machine learning principles.

The author is now revisiting and enhancing the project while completing the [Google Data Analytics Professional Certificate](https://grow.google/dataanalytics/). This updated version applies best practices learned from the course, including improved data cleaning, visualization, and analysis techniques.

---

## **Project Objectives**

- Highlight personal growth in data analysis and data science.
- Apply best practices from the Google Data Analytics Professional Certificate.
- Provide a comparative view of the initial project versus the updated approach.

---

## **Dataset Attribution**

This project uses the **UCI Credit Card Default dataset**, which contains information about default payments, demographic factors, and financial details for credit card clients in Taiwan.

- **Direct Source**: [UCI Credit Card Default Dataset](http://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients)
- **License**: [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)
- **Accessed via**: Kaggle

The raw dataset is included in this repository under `data/raw/UCI_Credit_Card_original.csv`. Attribution is required for reuse. This dataset is distributed under the terms of the [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0/).

---

## **Current Progress**

The project currently includes:
1. **Raw Dataset**:
   - Directly downloaded from the UCI Machine Learning Repository.
2. **Cleaned Dataset**:
   - Features the latest cleaned version (`v5.0.0`) with:
     - Consolidated ambiguous values in the `EDUCATION` column into a single category (`Unknown`).
     - Converted numerical columns (`MARRIAGE`, `SEX`) into descriptive textual labels.
     - Added a new column `Pay Status Word` for clearer interpretation of `PAY_X` values.
     - Renamed `Pay Status` and `Pay Status Word` columns to include their corresponding months.
     - Reordered columns to reflect ascending chronological order (April 2005 to September 2005) instead of the original descending order.

---

## **Key Improvements**

- **Ambiguous Values**: Consolidated unknown values in the `EDUCATION` column for clarity.
- **Column Headers**: Renamed technical headers to user-friendly names (e.g., `PAY_X` → `Pay Status`).
- **Textual Labels**: Translated numerical values in columns like `SEX` and `MARRIAGE` into descriptive textual labels.
- **Chronological Order**: Reorganized columns to follow a logical, ascending timeline.
- **New Column**: Added `Pay Status Word` for verbal descriptions of payment status.

---

## **Progress and Changelog**

Detailed cleaning and transformation steps are documented in the [Changelog](changelog/UCI_Credit_Card_Changelog.md).

---

## **Visualizations (Coming Soon)**

Interactive and static visualizations showcasing the dataset's structure and key insights will be added to this repository. These will include:
## **Visualizations (Coming Soon)**

Interactive and static visualizations showcasing the dataset's structure and key insights will be added to this repository. These will include:

- **Distribution of Payment Status**:
  - Visualize how payment statuses are distributed across clients.
- **Trends in Bill Amounts and Payments Over Time**:
  - Highlight patterns and fluctuations in bill amounts and payments over the months.
- **Relationships Between Demographic Factors and Default Probabilities**:
  - Show how factors like education, marriage, and age influence the likelihood of defaulting.
- **Correlation Between History of Delinquency and Probability of Defaulting**:
  - Analyze how past payment behavior impacts the risk of future defaults.
- **Feature-to-Target Correlation**:
  - Identify the strongest predictors of default by comparing features to the target variable (`default_payment`).
- **Feature Correlation and Comparison**:
  - Explore relationships between features (e.g., bill amount vs. payment amount) to detect trends or dependencies.


---

## **Dataset Access**

A subset of the cleaned dataset is provided for quick access and review, ensuring smooth performance and easier navigation.

- **[View Subset of Cleaned Dataset on Google Sheets](https://docs.google.com/spreadsheets/d/e/2PACX-1vQWNZqWcxU6W3FpGr6osZGHQVhhg_5nsbwOSHLOi8-vMYSuPfecDDlyC_ZeRqHuvj4LD712mcnuOlr0/pubhtml#)**:
  - Contains the first 1,000 rows of the cleaned dataset (`v5.0.0`).
- **[Download Full Cleaned Dataset (CSV)](data/cleaned/UCI_Credit_Card_cleaned_v5_0_0.csv)**:
  - The complete cleaned dataset with all 30,000 rows.

---

## **Future Plans and Additions**

- Perform exploratory data analysis (EDA) to identify trends and correlations.
- Develop Tableau dashboards for interactive visualization.
- Apply machine learning models to predict credit default risk.
- Include advanced visualizations and insights based on the cleaned dataset.
- Showcase results from an initial machine learning model using the prepared data.

---

## **Contact**

For inquiries or collaboration, feel free to reach out:
- **Author**: Johnpaul Medina
- **Email**: [jmedinacs715@gmail.com](mailto:jmedinacs715@gmail.com)
- **GitHub Profile**: [https://github.com/jmedinacs](https://github.com/jmedinacs)
