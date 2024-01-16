# Bangalore House Price Prediction

## Overview

This repository contains a K Nearest Neighbor (KNN) regressor model implemented in Python using Jupyter Notebook to predict the price of houses in Bangalore. The project follows the complete machine learning lifecycle, covering data cleaning, analysis, visualization, model creation, and evaluation.

## Data Cleaning

During the data cleaning phase, several issues were identified and addressed:

- The data types of 'bath' and 'balcony' were floating-point, even though their values cannot be decimal. The 'bath' column was changed to integer values, and records with decimal values in the 'balcony' column (2.83% of total records) were excluded.

- Inappropriate and lengthy column names were renamed for better readability.

## Data Analysis and Visualization

Insights were derived from the data analysis and visualization process:

- 'total_sqft' demonstrated a strong correlation with 'price,' while 'bath' and 'bhk' exhibited moderate correlations with 'price.' Other variables showed weak correlations.

- The majority of houses consisted of 2 BHK, followed by 3 BHK. However, the highest average price per sqft was associated with 6 and 5 BHK.

- Houses with 3 balconies had the highest average price per sqft, followed by those with no balconies.

- 'Super built-up area' was the most common area type, but 'plot area' had the highest average price per sqft.

- Houses with 'ready to move' availability had a higher count, but the average price per sqft was nearly the same for both types.

- The top-priced and bottom-priced locations were displayed.

## KNN Regressor Model

The KNN regressor model was created using the sklearn library. Grid search with cross-validation was employed to evaluate different k values, and the model with k = 19 demonstrated the best performance.

## Model Evaluation

The KNN regressor model was evaluated using the following metrics:

- Mean Absolute Error: 4.4
- Mean Squared Error: 2742.91
- Root Mean Squared Error: 52.37

These metrics provide an understanding of the model's accuracy and effectiveness in predicting house prices.
