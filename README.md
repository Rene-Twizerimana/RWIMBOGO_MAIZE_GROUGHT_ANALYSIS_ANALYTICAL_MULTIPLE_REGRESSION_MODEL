**Drought Impact & Strategy Effectiveness Modeling for Maize Production (Rwimbogo, Rwanda)**

This repository contains a complete data science pipeline that analyzes how drought affects maize yield and how farmers’ coping strategies and institutional support reduce these losses.

The project includes:

Real-world-inspired agricultural, rainfall, and survey data

Data preprocessing & feature engineering

Correlation analysis

Two multiple regression models:

Model 1: Drivers of maize yield loss

Model 2: Drivers of strategy effectiveness

Model diagnostics & visualizations

The goal is to quantify climate vulnerability and measure the impact of adaptation strategies using interpretable econometric models.

** Problem Statement**

Farmers in drought-prone areas face repeated crop losses. However, not all farmers are affected equally. Some adopt strategies (e.g., drought-resistant seeds, irrigation), and some receive support (inputs, training, credit).

This project answers:

What factors increase maize yield loss?

What factors reduce maize yield loss?

Which factors make coping strategies more effective?


Modeling Approach
Step 1: Data Preparation

Multiple datasets were merged and transformed into quantitative indices:

Feature	Description
Drought_Frequency_Score	How often droughts occur
Drought_Effects_Score	Severity of drought impacts
Strategy_Adoption_Score	Level of coping strategy use
Support_Access_Score	Access to inputs, training, credit
Strategy_Effectiveness_Score	Perceived impact of strategies
Yield_Loss_Percentage	% maize yield loss (target)
Step 2: Correlation Analysis

Pearson correlation was used to:

Explore relationships

Check expected directions

Identify important predictors

Detect multicollinearity

Step 3: Regression Models
🔹 Model 1: Yield Loss Drivers (Main Model)

Predicts:

Yield_Loss_Percentage


Using:

Drought_Frequency_Score

Drought_Effects_Score

Strategy_Adoption_Score

Support_Access_Score

This is the core model of the project.

🔹 Model 2: Strategy Effectiveness Drivers

Predicts:

Strategy_Effectiveness_Score


Using:

Strategy_Adoption_Score

Support_Access_Score

Drought_Frequency_Score

Drought_Effects_Score

 **Model Evaluation**

Models are evaluated using:

Metric	Meaning
R²	Variance explained
Adjusted R²	Penalized R²
RMSE	Prediction error
MAE	Average absolute error

The main selection metric is R².

**VISUAL OUTPUTS**

The project generates:

Correlation heatmaps



**Methodology**

This project follows a structured data science workflow:

Data Collection & Integration

Agricultural production data

Rainfall and drought indicators

Farmer survey responses

Data Cleaning & Preprocessing

Handling missing values

Normalizing variables

Feature engineering

Creating composite drought and strategy indices

**Exploratory Data Analysis (EDA)**

Summary statistics

Distribution plots

Correlation analysis

Modeling

Multiple Linear Regression

Separate models for yield loss and strategy effectiveness

Model Evaluation

R²

Adjusted R²

RMSE

MAE

**Models Used**
**Model 1: Yield Loss Drivers (Main Model)**

Target variable:

Yield_Loss_Percentage

Predictors:

Drought_Frequency_Score

Drought_Effects_Score

Strategy_Adoption_Score

Support_Access_Score

This model identifies the main factors that increase or reduce maize yield loss.

**Model 2: Strategy Effectiveness Drivers**

Target variable:

Strategy_Effectiveness_Score

Predictors:

Strategy_Adoption_Score

Support_Access_Score

Drought_Frequency_Score

Drought_Effects_Score

This model explains what makes drought coping strategies more effective.

**Evaluation Metrics**

The models are evaluated using the following metrics:

Metric	Description
R²	Measures how much variance is explained by the model
Adjusted R²	Penalizes unnecessary predictors
RMSE	Measures average prediction error
MAE	Measures average absolute error

These metrics help assess both accuracy and generalization performance.

**Key Research Questions**

This project answers:

What factors increase maize yield loss under drought?

What factors reduce maize yield loss?

How effective are adaptation strategies?

What role does institutional support play?

Actual vs predicted plots

Residual diagnostics

Coefficient bar charts

Strategy vs loss trends
