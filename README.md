# zillow

This is the outline of the machine learning pipeline I used for reaching 95th place (top 4%) in kaggle's [Zillow Home Value Prediction Competition](https://www.kaggle.com/c/zillow-prize-1).

This is a three-level stacking model. The first two levels are xgboost and lightgbm, while the last level is simple weighted mean. All training and stacking are done with K-fold cross-validation to minimize information leakage. Feature engineering and parameter tuning are performed probabilistically through [Bayesian optimization](https://github.com/fmfn/BayesianOptimization/tree/master/bayes_opt).