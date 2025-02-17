# Changelog: UCI Credit Card Default Dataset

This document tracks the cleaning, validation, and transformation steps applied to the dataset as part of the author's data analysis journey.

| **ID** | **Category**  | **Description**                                                                                      | **Result**                                                                                       | **Date**    | **Version** | **Status**    |
|--------|---------------|------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|------------|-------------|---------------|
| 1      | Validate      | Checked for missing or blank data in all columns.                                                   | No missing or blank data found in any column.                                                  | 1/20/2025  | v1.0        | Completed     |
| 2      | Remove        | Checked for duplicates and removed any found.                                                       | No duplicates were found or removed.                                                          | 1/20/2025  | v1.0        | Completed     |
| 3      | Change        | Consolidated education levels.                                                                      | Merged `0`, `5`, and `6` into a new category `5` ("Unknown"). Updated 344 values.               | 1/20/2025  | v2.0        | Completed     |
| 4      | Validate      | Verified `Sex` column for valid entries.                                                            | All values confirmed as `1` (Male) or `2` (Female).                                            | 1/21/2025  | v2.0.1      | Completed     |
| 5      | Validate      | Created a tracking sheet for removed items.                                                        | A sheet was created to track removed or consolidated rows (e.g., Education `6` and `0`).       | 1/21/2025  | v2.0.2      | Completed     |
| 6      | Change        | Added `Cleaned Marriage` column.                                                                    | Converted numerical `MARRIAGE` data into descriptive labels: `0 = Unknown`, `1 = Married`.     | 1/21/2025  | v2.1.2      | Completed     |
| 7      | Delete        | Removed the original `MARRIAGE` column.                                                             | The original column was removed after creating the `Cleaned Marriage` column.                 | 1/21/2025  | v2.1.3      | Completed     |
| 8      | Change        | Updated column headers for clarity.                                                                 | Renamed columns (e.g., `PAY_X`, `BILL_AMT`, `PAY_AMT`) to more descriptive headers.            | 1/21/2025  | v2.2.3      | Completed     |
| 9      | Research      | Investigated undocumented `Pay Status` values (`0` and `-2`).                                       | Found references indicating `-2 = No Payment Required` and `0 = Minimum Payment Made`.         | 1/22/2025  | v2.2.3      | Completed     |
| 10     | Change        | Translated `Pay Status` values into verbal descriptions.                                             | Added `Pay Status Cleaned` column with labels: `-2 = No Payment Required`, `0 = Minimum`.      | 1/22/2025  | v2.3.3      | Completed     |
| 11     | Evaluate      | Analyzed distribution of `Pay Status` values.                                                       | Found 81% of data has `Pay Status = 0`, while statuses `3+` only make up 2%.                   | 1/25/2025  | v2.3.3      | Completed     |
| 12     | Change        | Translated `EDUCATION` values into descriptive labels.                                               | Updated values: `1 = Graduate School`, `2 = University`, `3 = High School`, `4 = Other`.       | 1/25/2025  | v3.3.3      | Completed     |
| 13     | Change        | Translated `Sex` values into descriptive labels.                                                    | Updated values: `1 = Male`, `2 = Female`.                                                     | 1/25/2025  | v4.3.3      | Completed     |
| 14     | Change        | Renamed `Pay Status`, `Bill`, and `Payment` columns to reflect months instead of numerical codes.    | Updated column names for clarity (e.g., `Pay Status 0` → `Pay Status September 2005`). Reordered columns in ascending order. | 1/26/2025  | v5.0.0      | Completed     |
| 15	 | Validate      | Created a Range Check sheet for Numerical Columns													| Verified minimum and maximum values for numerical columns. Identified possible outliers in billing and payment amounts. Observed negative balances, which require further investigation.| 1/26/2025 | v5.1.0 | Completed     |
| 16     | Validate      | Created Cleaning Investigations Sheet and consolidated cleaning documentation.             | Range check and negative bill amount investigation incorporated.                          | 1/27/2025   | v5.1.0      | Completed     |
| 17     | Validate      | Negative values for bill amount investigation.                                             | Age range within normal range. Pay status range within set parameters. Bill and payment amounts show negative and high values, candidates for further exploration and investigation. | 1/27/2025   | v5.1.1      | Completed     |
| 18     | Change        | Verbal Data Trimming.                                                                      | Trimmed all verbal columns to remove leading, trailing, and repeated spaces.              | 1/27/2025   | v5.1.2      | Completed     |
| 19     | Validate      | High `Bill` and `Payment` Amount Investigated.                                             | Analyzed customers' data that contain high `Bill` and `Payment` and confirmed that the amounts correspond to customer charging and payment behavior. Values were found appropriate and realistic.      | 1/29/2005 | v5.1.2      | Completed      |

---

## Key Observations

- The dataset initially contained ambiguous values in columns such as `EDUCATION` and `SEX`, which were consolidated for clarity.
- Severe class imbalance observed in `Pay Status`, with 81% of entries falling into `0` (Minimum Payment Made).
- All cleaning and transformation steps are tracked to ensure transparency and reproducibility.
- Pay status starts with 0 while BILL_AMT` and PAY_AMT` starts with 1. Also, dataset documentation indicates the months are in descending order Sept 2005 to April 2005.
- Minimum and Maximum range checked. `Age` and `Pay Status` are both wihtin normal range. `BILL_AMT` shows high values and negative values, flagged for further investigation.
- Further investigation of negative values in `BILL_AMT` likely due to customer overpayment, verified through comparison of `BILL_AMT` and `PAY_AMT`. 
- Granular data about `BILL_AMT` and `PAY_AMT` can yield more definitive data about the negative amount but taht data is not within this dataset. 

---

## Future Plans

1. Apply advanced visualization techniques to showcase trends and correlations.
2. Perform exploratory data analysis (EDA) to identify hidden patterns in the data.
3. Transition to machine learning modeling to predict default probabilities.
