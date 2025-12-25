# Mark Analyzer

**Predictive Analysis of Student Marks Using Historical Board Data (Pakistan)**

---

## Purpose

We believe that deep, data-driven understanding of student performance can inform better educational decisions, policy analysis, and academic planning.

---

## Approach

This project aimed to analyze historical examination results from **BISE Lahore** and the **Federal Board of Pakistan** using statistical learning techniques to:

-   Identify structural patterns in marks
-   Measure board-wise and year-wise variance
-   Evaluate predictability under realistic assumptions

---

## Outcome

The intended outcome was a predictive model capable of estimating student marks using variables such as:

-   Examination board
-   Academic year
-   Subject group
-   Location and school metadata (where available)

---

## Project Status ⚠️

**Paused — Data Inconsistency Identified**

During exploratory data analysis and preprocessing, significant structural inconsistencies were found across datasets, including:

-   Non-uniform grading schemes
-   Missing or unreliable metadata
-   Inconsistent subject mappings across years
-   Schema drift between boards and result formats

These issues invalidate key model assumptions and risk misleading results.  
The project was intentionally halted rather than forcing unreliable predictions.

> **Stopping was a design decision, not a failure.**

---

## Intended Model Design

-   **Model:** Linear Regression
-   **Inputs:** Historical marks, board, year, subject group, optional metadata
-   **Outputs:**
    -   Predicted marks
    -   Error metrics (RMSE, R²)
    -   Confidence intervals
-   **Analysis:**
    -   Board-wise bias
    -   Year-wise drift
    -   Error distribution and residual diagnostics
-   **Feature Selection:** `sklearn.feature_selection`

---

## Core Assumptions

-   Historical performance contains predictive signal
-   Marking schemes remain mostly stable
-   Feature–mark relationships are approximately linear
-   Random noise exists but is non-adversarial
-   Training data is representative of future data

---

## Explicit Non-Assumptions

-   Does not predict intelligence, effort, or potential
-   Does not guarantee individual outcomes
-   Does not infer causation from correlation
-   Does not model psychological, social, or behavioral factors

---

## Key Learnings

-   Real-world educational data is messy by default
-   Schema stability matters more than model choice
-   Bias can be structural, not statistical
-   Early termination can be the most rigorous outcome
-   Data quality defines the ceiling of any model

---

## Success Criteria (Original)

-   **Minimum:** No data leakage; R² > 0
-   **Strong:**
    -   Stable predictions across boards and years
    -   Interpretable feature coefficients
    -   Transparent error analysis

These criteria could not be met reliably under current data conditions.

---

## Notes

-   Independent side project for learning and experimentation
-   Focused on analysis and insight, not production deployment
-   Repository retained for:
    -   Data inspection
    -   Methodology reference
    -   Future resumption if higher-quality data becomes available

---

## Closing Statement

This project demonstrates a key principle of applied machine learning:

> **Prediction is only as good as the features available.**

Future work may resume if datasets include sufficient contextual features such as school, location, subject-level history, and other relevant metadata.
