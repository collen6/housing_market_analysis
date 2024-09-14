# housing_market_analysis
Project Overview
This project, titled Housing Market Analysis Project, aims to analyze the factors that influence housing prices in King County, Washington. The analysis focuses on two primary questions:

What internal housing factors influence the price of homes?
Does the presence of categorical variables like Waterfront, Condition, View, Grade, Year Built, and Year Renovated increase the likelihood of a house being sold above the median price?
The project employs multiple linear regression and logistic regression models to determine the internal and external factors influencing housing prices. Data is sourced from a publicly available King County housing dataset.

This project demonstrates essential data science skills including:

Data Preprocessing and Wrangling: The project involves handling a large dataset from the King County housing market, with cleaning, transformation, and creation of new variables for more meaningful analysis. The data preprocessing steps include handling missing data, transforming categorical and numerical variables, and creating new features based on domain knowledge.

Exploratory Data Analysis (EDA): The project thoroughly explores the dataset using visualizations (histograms, scatter plots, correlation matrices, etc.) to identify relationships between variables such as price, square footage, and condition. This skill is crucial for uncovering patterns and insights from raw data.

Statistical Modeling: The analysis leverages multiple linear regression to predict housing prices based on various features. Logistic regression is also used to predict whether a house sells above the median price, incorporating categorical and numerical variables. The project includes model selection processes (e.g., forward selection, backward selection) and testing model assumptions.

Feature Engineering: Feature creation and transformation play a key role in improving model performance. The project engineers new variables such as indicator variables for categorical data (e.g., condition, view) and creates decade-based groupings for continuous variables like year built and year renovated.

Model Evaluation: The project evaluates model performance using metrics such as R-squared, root mean square error (RMSE), precision, and accuracy. This involves comparing models through techniques like ANOVA F-tests, residual analysis, and multicollinearity checks (using Variance Inflation Factors).

Data Visualization: A key component of the analysis is effective communication through data visualization. Using tools like ggplot2, the project produces clear and insightful graphs (box plots, scatter plots, density plots) that help explain relationships between variables and support findings.

Model Selection and Optimization: The project applies model selection techniques (stepwise regression, AIC-based model comparison) to identify the best predictors for housing prices and optimize the model for better performance.

Handling Multicollinearity: The project assesses and addresses multicollinearity by examining correlations between variables and applying techniques like Variance Inflation Factor (VIF) calculations, ensuring the final models are robust and interpretable.

Statistical Hypothesis Testing: Hypothesis testing is performed to validate the significance of predictors. This skill shows an ability to test the validity of models and ensure the right variables are included for accurate predictions.

These skills—ranging from data wrangling, feature engineering, statistical analysis, and model evaluation—demonstrate the competencies employers seek in data scientists who need to analyze complex datasets and develop predictive models that lead to actionable insights.

Data Description
The dataset used for the analysis consists of housing data from King County, Washington, including homes sold between May 2014 and May 2015. The dataset contains 21 variables, of which 13 are directly used in the models, and 6 additional variables are created for further analysis.

Key variables include:

price: Sale price of the house (response variable)
bedrooms: Number of bedrooms
bathrooms: Number of bathrooms
sqft_living: Square footage of the interior living space
waterfront: Binary indicator for whether the house is near a waterfront
view: Rating of the view (0-4)
condition: Rating of the condition (1-5)
grade: Construction and design grade (1-13)
yr_built: Year the house was built
yr_renovated: Year the house was last renovated
Project Structure
Housing Market Analysis Project.Rmd: This is the main R Markdown file that contains the data preprocessing, analysis, and visualization. The file provides step-by-step insights into the study's methodology, results, and conclusions.

Housing Market Analysis Project.pdf: The compiled report in PDF format. It summarizes the entire analysis, including data exploration, model fitting, and findings.

Analysis
Question 1: Internal Factors Influencing Price
The team initially considered several internal features such as the number of bedrooms, bathrooms, floors, living space, and condition. Through model selection, the most significant predictors were narrowed down to:

Square footage of living space: Larger houses are priced higher.
Construction grade: High-quality construction and design also significantly increase house prices.
Question 2: Predicting Sale Above Median Price
Using logistic regression, the project evaluates whether a house sells above the median price ($450,000). The key predictors identified for this model include:

Condition: Houses in better condition are more likely to sell above the median price.
View: Houses with a better view are more likely to be priced higher.
Year Built: Newer houses have a higher likelihood of being sold above the median price.
Year Renovated: Recently renovated houses also tend to be priced above the median.
Waterfront: Proximity to a waterfront increases the chances of a higher price.
Key Findings
Square footage and grade are the most significant internal predictors of house prices.
Condition, view, and renovation year are critical categorical variables that influence whether a house sells above the median price.
Houses near a waterfront are generally more expensive, but this factor is not as significant in the final logistic regression model.
How to Use This Repository
Download the dataset: The dataset used is publicly available from Kaggle. Please download the King County Housing Prices dataset from Kaggle.

Run the analysis: Open the Housing Market Analysis Project.Rmd file in RStudio. This file walks you through the data preprocessing, exploratory analysis, model fitting, and conclusions.

View the results: The Housing Market Analysis Project.pdf contains the complete report and visualizations of the analysis.

Required Libraries
tidyverse: Data manipulation and visualization
MASS: For model fitting
caret: Used for model evaluation
ggplot2: For creating visualizations
dplyr: Data wrangling
leaps: For model selection
Conclusion
The analysis presented in this project is an insightful look into the King County housing market, revealing how internal housing features and categorical variables impact house prices. The findings are useful for homeowners, real estate professionals, and investors looking to make data-driven decisions in the housing market.

Author
Christian Ollen
Stat 6021, Project 2
