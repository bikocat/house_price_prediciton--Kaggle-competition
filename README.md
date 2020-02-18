# house_price_prediciton: Kaggle competition
 House price regression using lasso method

## Data manipulation:

-Removed variables with more than 90% of Nas
-Imputation of Nas with 0  or None (for categorical) in the case it stays for the absence of the feature in the corresponding observation  -Imputation of NAs with most frequent terms (mode function) for some features
-Imputation Lot frontage Nas with median grouped by Neighborhood
-Removed variable Utilities
-log trasform of SalePrice and other skewed numeric features
-use dummyVars caret libray to encode categorical variables

## Model selection:
-Lasso with cross-validation (10 kfold) glmnet library

Kaggle score: 0.12229

## Data manipulation
-perform a  linear regression over all data to detect outliers with function OutliersTest()
-perform a  linear regression over the important feature GrLivArea
-Model selection
-Lasso with cross-validation (10 kfold)  glmnet library

Kaggle score: 0.11777

## Data manipulation and Features engeneering
-new feature: TotalFeet (TotalBsmtSF+X1stFlrSF+X2ndFlrSF)
-new feature:  Grg binary variable to represent presence/absence
-new features:  squared-root of the age of the garage and of the house
-transform   numeric feature “OverallQual”  in to categorical



