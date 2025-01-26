# Changelog: UCI Credit Card Default Dataset

This document tracks the cleaning, validation, and transformation steps applied to the dataset as part of the author's data analysis journey.

| **ID** | **Category**  | **Description**                                                | **Result**                                                                                       | **Date**    | **Version** | **Status**    |
|--------|---------------|----------------------------------------------------------------|-------------------------------------------------------------------------------------------------|------------|-------------|---------------|
| 1      | Validate      | Checked for missing or blank data in all columns.             | No missing or blank data found in any column.                                                  | 1/20/2025  | v1.0        | Completed     |
| 2      | Remove        | Checked for duplicates and removed any found.                 | No duplicates were found or removed.                                                          | 1/20/2025  | v1.0        | Completed     |
| 3      | Change        | Consolidated education levels.                                | Merged `0`, `5`, and `6` into a new category `5` ("Unknown"). Updated 344 values.               | 1/20/2025  | v2.0        | Completed     |
| 4      | Validate      | Verified `Sex` column for valid entries.                      | All values confirmed as `1` (Male) or `2` (Female).                                            | 1/21/2025  | v2.0.1      | Completed     |
| 5      | Validate      | Created a tracking sheet for removed items.                  | A sheet was created to track removed or consolidated rows (e.g., Education `6` and `0`).       | 1/21/2025  | v2.0.2      | Completed     |
| 6      | Change        | Added `Cleaned Marriage` column.                              | Converted numerical `MARRIAGE` data into descriptive labels: `0 = Unknown`, `1 = Married`.     | 1/21/2025  | v2.1.2      | Completed     |
| 7      | Delete        | Removed the original `MARRIAGE` column.                       | The original column was removed after creating the `Cleaned Marriage` column.                 | 1/21/2025  | v2.1.3      | Completed     |
| 8      | Change        | Updated column headers for clarity.                           | Renamed columns (e.g., `PAY_X`, `BILL_AMT`, `PAY_AMT`) to more descriptive headers.            | 1/21/2025  | v2.2.3      | Completed     |
| 9      | Research      | Investigated undocumented `Pay Status` values (`0` and `-2`). | Found references indicating `-2 = No Payment Required` and `0 = Minimum Payment Made`.         | 1/22/2025  | v2.2.3      | Completed     |
| 10     | Change        | Translated `Pay Status` values into verbal descriptions.       | Added `Pay Status Cleaned` column with labels: `-2 = No Payment Required`, `0 = Minimum`.      | 1/22/2025  | v2.3.3      | Completed     |
| 11     | Evaluate      | Analyzed distribution of `Pay Status` values.                 | Found 81% of data has `Pay Status = 0`, while statuses `3+` only make up 2%.                   | 1/25/2025  | v2.3.3      | Completed     |
| 12     | Change        | Translated `EDUCATION` values into descriptive labels.         | Updated values: `1 = Graduate School`, `2 = University`, `3 = High School`, `4 = Other`.       | 1/25/2025  | v3.3.3      | Completed     |
| 13     | Change        | Translated `Sex` values into descriptive labels.              | Updated values: `1 = Male`, `2 = Female`.                                                      | 1/25/2025  | v4.3.3      | Completed     |

---

## Key Observations

- The dataset initially contained ambiguous values in columns such as `EDUCATION` and `SEX`, which were consolidated for clarity.
- Severe class imbalance observed in `Pay Status`, with 81% of entries falling into `0` (Minimum Payment Made).
- All cleaning and transformation steps are tracked to ensure transparency and reproducibility.

---

## Future Plans

1. Apply advanced visualization techniques to showcase trends and correlations.
2. Perform exploratory data analysis (EDA) to identify hidden patterns in the data.
3. Transition to machine learning modeling to predict default probabilities.
