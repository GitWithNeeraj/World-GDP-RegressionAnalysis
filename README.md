# World-GDP-RegressionAnalysis
Analyzing the World GDP data from the World BanK to estimate the long-term annual growth rate of the world using regression techniques
# World GDP Analysis

## Project Overview
This project involves analyzing the World GDP data from the World Bank. The aim is to estimate the long-term annual growth rate of the world using regression techniques. 

## Problem Statement
The task is to download and analyze the World GDP data. The specific objectives are:
- Apply a logarithmic transformation to linearize the exponential growth of GDP over time.
- Perform a linear regression on the transformed data and plot the results.
- Compute and analyze the residuals of the regression.
- Conduct a Kolmogorov-Smirnov test to examine the distribution of the residuals.
- Apply the inverse transformation to the regression model and compare it with the original GDP data.
- Calculate the long-term growth rate of the World GDP and analyze trends post-2015.

## How to Run
Ensure you have Jupyter Notebook installed with numpy, matplotlib, scipy, and pandas-datareader.

1. Clone this repository.
2. Navigate to the repository directory.
3. Open `data_analysis.ipynb` in Jupyter Notebook.
4. Run the cells to see the analysis and results.

## Dependencies
- numpy
- matplotlib
- scipy
- pandas-datareader


world GDP time series

![image](https://github.com/GitWithNeeraj/World-GDP-RegressionAnalysis/assets/84373485/cbafed09-03e9-48a8-b2a6-2dd5b65c6a2d)
![image](https://github.com/GitWithNeeraj/World-GDP-RegressionAnalysis/assets/84373485/0866d212-fe61-4a43-b90e-121c255a6bb7)
The p-value we got is less than 0.01. So, we can reject the null hypothesis that that the residuals are sampled from a normal distribution.

The inverse transformation of logarithm is exponent. So, we apply the exponent operation to our linear model.

From 2015, the prediction of our model does not match with the actual gdp. Because, according to the our model, the rate of increase is greater than the actual increase in gdp data. Intuitively this makes sense as we would not expect gdp to increase at such a rapid rate.
![image](https://github.com/GitWithNeeraj/World-GDP-RegressionAnalysis/assets/84373485/fc5405e4-70e9-4b40-9b99-1771fad348ee)
