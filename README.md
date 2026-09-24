### About

This is an income statement projections project using a sample 2021 income statement created by the [Actuarial Accelerator Community](https://etchedactuarial.com/accelerator) for educational purposes.

This project aims to do the following:

**1. Project the net income for the years 2022-2025, given assumptions about the annual changes in each component of revenue and expenses.**

This is implemented in `income statement projections.xlsm`, which contains the following worksheets:
- **2021 Income Statement**: The sample 2021 income statement.
- **Income Projections**: The calculator for the net income projections from the 2021 income statement, which uses inputs regarding the rate change and its direction (increase or decrease) for each component of revenue and expenses, as well as the interest rate, which affects the rate change of each component in the following way:
    - If interest rate are 2-4% (inclusive), then the annual change assumptions for
        - Investment Income: decrease by 0.25% (multiplicatively)
        - Gross Claims: increase by 1% (multiplicatively)
        - Change in Insurance Liabilities: increase by 1.5% (multiplicatively)
        - Equipment Expenses: increase by 2% (multiplicatively)
    - If interest rate are 5-7% (inclusive), then the annual change assumptions for
        - Investment Income: increase by 0.625% (multiplicatively)
        - Gross Claims: decrease by 0.7% (multiplicatively)

**2. Compute the total net income for the years 2022-2025 for 100 different scenarios of annual changes, accounting for interest rates of 2%, 4%, 6%, and 8%.**

This is implemented in `total net income for forecasting data scenarios.xlsm`, using macros. Note that in order to run these macros, ensure that macros are enabled for this file and that `income statement projections.xlsm` is opened as well.