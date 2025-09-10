# Fertilizer Predictions - kNN Classification
**Course:** _DA5030 - Introduction to Machine Learning & Data Mining_

## Overview
This project utilizes kNN classification to train a model to predict the type of fertilizer based on the climate and soil conditions.
This project follows the CRISP-DM framework, and the final output is a reproducible R Notebook report combining narrative, analysis, and code.

## Data
The data is loaded into separate dataframes using their URLs:
* _Training Data_: [`fertilizer-recommendation.csv`](https://s3.us-east-2.amazonaws.com/artificium.us/datasets/fertilizer-recommendation.csv)
* _Validation Data_: [`fertilizer-recommendation-validation.csv`](https://s3.us-east-2.amazonaws.com/artificium.us/datasets/fertilizer-recommendation-validation.csv)

## Deliverables
* `fertilizer_recommendation.Rmd` - R Notebook
* `fertilizer_recommendation.html` - knitted HTML report
* `fertilizer-recommendation-validation-predicted.csv` - predictions for the validation dataset

## Dependencies
* dplyr
* caret
* kableExtra
* class
* gmodels

## Methodology
1. Load Data
2. Explore Data
3. Shape Data for kNN
   * Identify predictors
   * Encode categorical variables
   * Scale data
   * Create training/testing sets
4. Train and Tune kNN
5. Validate Model

## Results
The final predictions for the validation data are saved in `fertilizer-recommendation-validation-predicted.csv`.  
This file:  
- Includes headers and no row numbers  
- Preserves the original order of the validation dataset  
- Contains two columns: **X** (observation ID) and **Fertilizer**  

The full analysis and visualizations are available in the [knitted report](https://zoechow24.github.io/fertilizer-kNN-prediction/fertilizer_recommendation.html).

