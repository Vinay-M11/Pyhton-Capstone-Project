# Capstone Project: Python Fundamentals

This repository contains the deliverables for the **SkillVilla Python Fundamentals Capstone Project**. The primary objective of this project is to demonstrate core data manipulation, cleaning, and preprocessing skills using **Python**, **Pandas**, and **NumPy**. 

The project evaluates real-world data engineering scenarios including handling missing values, joining multiple relational datasets, feature engineering, conditional updates, and string manipulation.

---

## 📊 Dataset Overview

The project processes three distinct dataframes containing relational project and organizational data:

1. **Employee DataFrame**: Tracks general employee demographics (`ID`, `Name`, `Gender`, `City`, `Age`).
2. **Seniority Level DataFrame**: Maps employees to their current position grade (`ID`, `Designation Level` on a scale of 1 to 4).
3. **Project DataFrame**: Tracks project financial metrics and execution statuses (`ID`, `Project`, `Cost`, `Status`).

---

## 🛠️ Task Breakdowns

The project consists of 10 sequential operational tasks executed inside a Jupyter Notebook:

*   **Task 1: Data Initialization** – Programmatically build the base DataFrames and export them into standalone `.csv` files for downstream consumption.
*   **Task 2: Imputation via Running Average** – Handle missing project financial records in the `Cost` column by computing and filling values using a custom `for` loop implementation.
*   **Task 3: Text Processing & Name Splitting** – Parse full names into independent `First Name` and `LastName` features while dropping the legacy column.
*   **Task 4: Relational Database Joins** – Merge all three localized datasets into a single, comprehensive master dataframe named `Final`.
*   **Task 5: Financial Feature Engineering** – Generate a conditional `bonus` metric awarding a 5% allocation relative to project costs exclusively to completed operations.
*   **Task 6: Organizational Demotions & Compliance Filtering** – Penalize performance by downgrading the designation tier for failed operations and filtering out records that fall below organization thresholds (level > 4).
*   **Task 7: Salutation Formatting** – Transform structural strings by prepending gender-appropriate titles (`Mr.` / `Mrs.`) to the employee names and purging redundant demographic columns.
*   **Task 8: Conditional Promotions** – Apply localized conditional logic via `if` conditions to advance structural seniority rankings for experienced resources over 29 years old.
*   **Task 9: Cost Aggregations** – Aggregate individual financial commitments to generate a high-level summary dataframe named `TotalProjCost`.
*   **Task 10: String Pattern Filtering** – Query and extract complete employee metrics based on specific geographical string matches (cities containing the letter "o").

---

## 🚀 Technologies & Environment

*   **Language:** Python 3.x
*   **Libraries Used:** Pandas, NumPy
*   **Environment:** Jupyter Notebook (`.ipynb`)

---

## 📁 Repository Structure

```text
├── data/
│   ├── employee.csv            # Generated Employee source data
│   ├── seniority_level.csv     # Generated Seniority level source data
│   └── project.csv             # Generated Project tracking data
├── capstone_notebook.ipynb     # Fully executed Jupyter Notebook with comprehensive comments
└── README.md                   # Project documentation
```

---

## 📈 Evaluation Deliverables
As per project requirements:
*   Every single line of code within the source `.ipynb` file is explicitly annotated with clear comments.
*   All intermediate processing steps and final outputs are preserved directly inside the notebook cells.
