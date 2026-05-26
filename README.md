# Stochastic Retirement Wealth & Pension Modeling Engine

A comprehensive financial modeling engine built in Excel to simulate long-term wealth accumulation and Account-Based Pension (ABP) drawdowns. This project utilizes Monte Carlo simulations and multi-variable sensitivity analysis to evaluate retirement portfolio longevity and probability of ruin.

## Project Structure
The underlying model (`Stochastic Retirement Modeling Engine.xlsx`) consists of six interconnected core modules:
1. **Inputs**: Dynamic dashboard configuring macroeconomic assumptions, wage growth, contributions, and initial capital parameters.
2. **Stochastic Rates**: Implementation of an Euler-Maruyama discretization scheme to generate 1,000+ random pathways for interest and inflation rates.
3. **Simulation Grid**: The core stochastic execution engine computing time-series projections for wealth accumulation.
4. **Summary & Analysis**: Statistical aggregation of simulation endpoints to calculate risk-return distributions and retirement adequacy.
5. **ABP Modeling**: Automated drawdown schedules integrating statutory minimum withdrawal percentages set by regulatory frameworks.
6. **Sensitivity Analysis**: Stress-testing engine evaluating portfolio longevity across varied volatility levels and fee structures.

## Methodology & Technical Features
* **Stochastic Rate Engine:** Transformed deterministic projections into a probabilistic framework by simulating correlated paths using an Euler-Maruyama discrete-time approximation.
* **Dynamic Drawdown Automation:** Modeled the Account-Based Pension (ABP) phase using conditional logic to enforce age-based statutory minimum drawdowns while dynamically tracking remaining capital.
* **Risk Quantification:** Aggregated Monte Carlo endpoints to output Value-at-Risk (VaR) and determine the exact statistical "Probability of Ruin" (the likelihood of outliving retirement savings).

## How to Use the Model
1. CDuplicate or download this repository.
2. Open `Stochastic Retirement Modeling Engine.xlsx` in desktop Microsoft Excel (ensure iterative calculations are enabled if prompted).
3. Modify the parameters in the `Inputs` tab to observe how the overall probability of ruin and pension longevity shift in real-time.
