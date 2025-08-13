# 🛢️ Oil Well Location Selection

## 📌 Project Overview

Helps oil company "GlavRosGosNeft" identify optimal drilling locations by analyzing geological data from three regions. The solution predicts oil reserves volume and evaluates financial viability to maximize profitability while minimizing investment risks.

## 🎯 Objective

Select the most profitable region for oil extraction by:
- Building accurate volume prediction models
- Identifying top 200 most promising wells from 500 surveyed locations
- Calculating potential profit and assessing risks using bootstrap analysis
- Ensuring risk of losses remains below critical 2.5% threshold

## 📊 Dataset Description

Three datasets with geological measurements for 10,000 wells per region:
- Technical features (f0, f1, f2) - geological measurements
- Target feature: product (oil reserves in thousand barrels)

## 🔍 Methodology

### Data Preparation
- Removed unnecessary ID column
- Split data into training and validation sets
- Applied linear regression models for each region

### Risk Assessment
- Budget constraint: 10 billion rubles
- Revenue model: 450,000 rubles per barrel
- Implemented bootstrap technique (1,000 iterations) to simulate profit distribution
- Calculated confidence intervals and loss probabilities

## 📈 Results

**Optimal Region**: Region 2

**Key Outcomes**:
- Highest prediction accuracy (significantly lower RMSE than other regions)
- Consistent profitability with only 0.3% risk of losses (well below 2.5% threshold)
- Positive profit in all bootstrap simulations
- 95% confidence interval entirely in positive territory

The analysis successfully identified Region 2 as the optimal choice for oil extraction, balancing high profitability with minimal financial risk, enabling confident investment decisions for the company.
