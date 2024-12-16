# IRR and XIRR Calculation and Visualization for Venture Capital Funds

This Python script calculates and visualizes the Internal Rate of Return (IRR) and Extended Internal Rate of Return (XIRR) for hypothetical venture capital (VC) funds. It is designed to help understand and compare different return metrics by showing how the Net Present Value (NPV) behaves in relation to different discount rates.

## Key Features

*   **NPV Calculation:** Calculates the Net Present Value (NPV) for different discount rates.
*   **IRR Calculation:** Computes the Internal Rate of Return (IRR) using both the `numpy_financial` and `scipy` libraries.
*   **XIRR Calculation:** Calculates the Extended Internal Rate of Return (XIRR) using `scipy.optimize` library, using specific dates for cash flows.
*   **Cash Flow Data:** Visualizes and prints the cash flows for different example funds
*   **Interactive Plot:** Generates an interactive graph using `matplotlib` to visualize the relationship between NPV and the discount rate, that allows the user to interact with it.
*   **Clear Output:** Provides clearly formatted tables and descriptive text to help understand the results, and gives a strong insight into what it is doing and how to read the information.

## How To Use

1.  **Install Requirements:** First, make sure you have the necessary libraries installed. You can usually use `pip install numpy numpy-financial matplotlib scipy tabulate`:
```bash
   pip install numpy numpy-financial matplotlib scipy tabulate
Use code with caution.

Copy and Paste or Clone: Copy or clone this file to your local environment.

Run the Script: Execute the Python script using:

python3 irr_xirr_fund_perf.py
Use code with caution.
Bash
View Results:

The script will first display a table showing the cash flows of the different funds you are testing.

It will then output the calculated IRR (using both numpy and scipy), and the calculated XIRR for each fund, as well as their corresponding NPV graph in a new window, which you can explore interactively.

Press "Enter" to close the plot window and conclude the script.

Understanding the Output
Table of Cash Flows
The table will show you the input data of your test. It has one line for each fund with the following data.

Fund The name of the tested fund (A, B or C).

Year 1, Year 2, etc The amount of the cash flow for the specific year.

IRR and XIRR Results
The output of the script will include:

IRR (numpy): The Internal Rate of Return calculated by numpy_financial.

IRR (scipy): The Internal Rate of Return calculated by scipy.optimize.

XIRR The eXtended Internal Rate of Return, considering the timing of the cashflows.

The NPV vs. Discount Rate Plot
The plot shows:

X-axis (Discount Rate): This shows the different discount rates being applied from -50% to 100% to calculate the Net Present Value.

Y-axis (Net Present Value): The NPV is the value of all discounted cashflows.

The lines: They each represents the evolution of the NPV as a function of the discount rate, for each of the funds that are being tested.

NPV = 0 Line: The horizontal dashed line represents zero NPV. The point where a given curve intercepts this line is the IRR for that specific fund.

How to Use this for Fund Benchmarking
By using this script and the resulting graph, you can better understand:

IRR: How do different cash flows impact the Internal Rate of Return.

XIRR: How do specific dates of cash flows impact the extended internal rate of return

NPV Sensitivity: By looking at the different curves, you will quickly visualize how a fund responds to changes in the discount rate (this shows the risk level of a given fund)

Comparing Returns: The IRR is a very useful metric to compare the returns and profitability of different funds.

Important: The examples provided are hypothetical, and you may need to tailor the code for your specific case.

Dependencies
Python 3.x

numpy

numpy_financial

matplotlib

scipy

tabulate

Disclaimer
Use this script at your own risk. The output of this script is for educational purposes.
