# Monte_-Carlo_-Portfolio_-Risk_-Simulator
# Monte Carlo Portfolio Risk Simulator — What If? Risk Lab

## Project Overview

The Monte Carlo Portfolio Risk Simulator is a beginner-friendly Python project that uses NumPy and Matplotlib to simulate possible portfolio outcomes and analyze investment risk.

The project generates 10,000 simulated portfolio paths over 252 trading days for four assets. It calculates portfolio volatility and estimates the 95% Value-at-Risk (VaR).

The project also includes a **What If? Risk Lab**, an additional feature that compares normal market conditions with hypothetical market-crash scenarios.

## Objectives

- Simulate daily returns for four assets.
- Generate 10,000 possible portfolio paths.
- Calculate cumulative portfolio values.
- Estimate annual portfolio volatility.
- Calculate 95% Value-at-Risk.
- Visualize simulated portfolio outcomes.
- Test the impact of hypothetical market crashes.
- Generate automatic risk reports.

## Technologies Used

- Python
- NumPy
- Matplotlib
- Google Colab

## Main Features

### 1. Asset Return Simulation

Uses `np.random.normal()` to generate simulated daily returns for four assets over 252 trading days.

### 2. Monte Carlo Portfolio Simulation

Generates 10,000 possible portfolio outcomes using NumPy arrays and matrix multiplication.

### 3. Portfolio Value Calculation

Uses `np.log1p()`, `np.exp()`, and cumulative returns to calculate simulated portfolio values over time.

### 4. Portfolio Risk Analysis

Calculates:
- Average final portfolio value
- Minimum and maximum final portfolio values
- Annual portfolio return volatility
- 95% Value-at-Risk (VaR)
- Probability of a profitable or loss-making outcome

### 5. Portfolio Visualization

Creates a histogram of final portfolio values and line graphs showing sample simulation paths.

## Innovative Features

### 6. What If? Market Crash Stress Test

This feature evaluates how a hypothetical sudden market decline may affect portfolio outcomes.

Three scenarios are compared:

- **Normal Market:** No additional shock.
- **Moderate Crash:** A hypothetical -5% shock.
- **Severe Crash:** A hypothetical -10% shock.

The shock is applied to all four assets on one simulated trading day. The project then compares average final portfolio values, estimated 95% VaR, and the probability of ending below the initial portfolio value.

### 7. Crisis Comparison Graph

A Matplotlib graph compares estimated portfolio risk under the three market scenarios, making differences easier to understand visually.

### 8. Automatic Risk Report

Generates a report for each scenario containing:
- Average final portfolio value
- Estimated 95% VaR
- Probability of a loss
- A simple rule-based risk alert

The risk-alert thresholds are illustrative and are not universal investment-risk standards.

### 9. Portfolio Allocation Comparison

Compares two hypothetical asset allocations:
- Equal-weight portfolio
- Alternative-weight portfolio

The project compares their simulated average final values and return volatility.

### 10. Final Risk Dashboard

Displays portfolio value distributions and scenario comparisons through graphs, making the simulation results easier to interpret.

## NumPy Concepts Used

- `np.array()`
- `np.random.seed()`
- `np.random.normal()`
- `np.mean()`
- `np.std()`
- `np.percentile()`
- `np.min()` and `np.max()`
- `np.sum()`
- `np.cumsum()`
- `np.log1p()`
- `np.exp()`
- Matrix multiplication using `@`
- Multidimensional NumPy arrays
- Boolean conditions and loops

## Matplotlib Concepts Used

- Histograms
- Line graphs
- Bar charts
- Axis labels and titles
- Legends
- Grid lines
- Multiple plots using subplots

## How to Run the Project

1. Open Google Colab.
2. Create a new Python notebook.
3. Copy each code block into a separate cell in the correct order.
4. Run all cells from top to bottom.
5. View the simulation results, risk reports, and graphs.

## Expected Output

- Simulated portfolio returns and paths
- Portfolio volatility and 95% VaR
- Best, average, median, and worst simulated outcomes
- Market-crash stress-test results
- Crisis comparison graph
- Automatic risk report
- Portfolio allocation comparison
- Final portfolio risk dashboard

## Limitations

This is an educational simulation, not a real investment forecasting tool. It uses hypothetical return assumptions and simplified market-crash scenarios. Asset returns are simulated independently, so real-world correlations, transaction costs, and changing market conditions are not fully represented.

The results should not be treated as financial advice or guarantees of future performance.

## Conclusion

The Monte Carlo Portfolio Risk Simulator demonstrates how NumPy and Matplotlib can be used to simulate possible portfolio outcomes, estimate financial risk, and visualize uncertainty.

Its What If? Risk Lab adds a practical scenario-testing feature, allowing users to compare hypothetical market conditions and understand how sudden shocks can affect simulated portfolio outcomes.

## Author

Created as a Python, NumPy, and Matplotlib learning project.
