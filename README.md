# House Prices | Machine Learning project
Predict sales prices using advanced regression techniques

**Data**: https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques 

**My attempt**: https://github.com/nganguyenny/Kaggle-House-Predict

### 1. Project Setup
- Load libraries
- Load datasets (upload datasets on GCP storage)
- Create scoring metric (rmsle)

### 2. Model Testing for Numeric Features
- Baseline score and RandomizedSearchCV searching for best params using:
- DecisionTreeRegressor, AdaBoostReegressor, GradientBoostingRegressor, XGBRegressor
- RandomForestRegressor (extracting feature importances)
- and stacking.

### 3. Baseline Pipeline
- Feature overview (numerical vs categorical features)
- Preprocessing (impute, scale, encode)
- Estimator (with DecisionTreeRegressor)
- Cross validation
- Prediction

### 4. Features Preprocessing
- Preprocessing: encoding (ordinal and nominal categorical features, numerical features, cyclical features), full preprocessing pipeline;
- Feature Investigation: numerical features (VIF to measure multicolinearity), ordinal features (spearman method), univariate feature selection (SelectPercentile)

### 5. Model Testing with All Features
- Data loading and target engineering
- Apply preprocessing pipeline
- Create RMSE score
- Linear models (LinearRegression, Ridge)
- KNeighborsRegressor, SVR,
- Trees (DecisionTreeRegressor),
- Random Forest (RandomForestRegressor),
- Boosteed Trees (AdaBoostRegressor, GradientBoostingRegressor),
- Stacking (VotingRegressor, StackingRegressor),
- XGBRegressor.

### 6. Kaggle Submission
- Best score using StackingRegressor (on test set locally): 0.12119
- Actual score valuated on Kaggle (top 12% on leaderboard): 0.12396
