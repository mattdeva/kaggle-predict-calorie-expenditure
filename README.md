# kaggle-predict-calorie-expenditure

Kaggle competition in the playground series which provides straightforward datasets and allows the community to practice machine learning techniques. In this May 2025 competition, the goal was to predict how many calories were burned during a workout. [Competition Overview](https://www.kaggle.com/competitions/playground-series-s5e5/overview)

Kaggle Notebook [My Notebook](https://www.kaggle.com/code/mattneel/calories-expenditure-modeling). This is not a comprehensive analysis, and there are many things to improve upon.

# Summary

The analysis includes several sections: EDA, creating a baseline model, feature engineering, residual analysis, new models, model comparison. I have summarized the milestones in each section:

Data
- Split data into train, validation, test
- Create visuals of feature distributions across datasets
- Visuals to examine feature to target relation to target

Baseline Model
- Sklearn column transformer to encode and normalize the data
- Fit basic LightGBM
- Use KFold cross validation

Feature Engineering
- Compute new features using existing features and my knwoledge of the subject
- Log transformations for some features in baseline

Residual Analysis
- Create visuals to demonstrate model trends and inefficiencies
- Analyze target distribution vs prediction distribution. Attempt weighting adjustment to potentially improve model.
- Create dataset and visuals of observations with most wrong predictions

New Modeling
- Updated LightGBM
- XGBoost (also using KFold)
- TensorFlow Neural Network

Modeling Comparison
- Compare target and prediction summary statistics in a table
- Compare competition target loss for each model and baseline
