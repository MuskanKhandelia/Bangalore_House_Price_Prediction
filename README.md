# Bangalore House Price Prediction and Analysis

## Overview

This repository contains code and analysis for predicting the price of houses in Bangalore using a K Nearest Neighbor (KNN) regressor model. The entire machine learning life cycle, including data cleaning, exploration, and model creation, has been implemented in Python using a Jupyter notebook.

## Data Cleaning

During the data cleaning process, the following issues were identified and addressed:

- 'bath' and 'balcony' columns had floating-point data types, even though their values cannot be decimal. The 'bath' column was converted to integer values. Records with decimal values in the 'balcony' column were excluded due to their insignificance.
- Inappropriate and lengthy column names were renamed for clarity.

## Data Analysis and Visualization

Insights were derived from data analysis and visualization using pandas and seaborn:

- 'total_sqft' demonstrated a strong correlation with 'price,' while 'bath' and 'bhk' exhibited moderate correlations.
- The largest proportion of houses consisted of 2 BHK, followed by 3 BHK. However, the highest average price per sqft was associated with 6 and 5 BHK, with 4 BHK following closely behind.
- Houses with 3 balconies had the highest average price per sqft, followed by those with no balconies.
- Most homes fell under the category of 'super built-up area,' yet the area type with the highest average price per sqft was 'plot area.'
- There were more houses with 'ready to move' availability, but the average price per sqft was nearly the same for both availability types.
- Top-priced and bottom-priced locations were displayed.

## KNN Regressor Model

A KNN regressor model was created using scikit-learn. As the sqrt of our training dataset was 74.43, considered 73 as the k value.

## Model Evaluation

The model was evaluated using the following metrics:

- Mean absolute error - 8.34
- Mean squared error - 4150.73
- Root mean squared error - 64.43

## Tableau Dashboard

A Tableau dashboard was created to provide visual insights into the Bangalore house price analysis.

![Dashboard 1](https://github.com/MuskanKhandelia/Bangalore_House_Price_Prediction/assets/65664089/bb16d355-13ce-4309-b8eb-1b3006ebceac)

https://public.tableau.com/views/Bangalore_House_Price_Analysis/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link
