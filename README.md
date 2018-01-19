# zillow

This is the outline of the machine learning pipeline I used for reaching 51th place (top 2%) in Kaggle's [Zillow Home Value Prediction Competition](https://www.kaggle.com/c/zillow-prize-1).

This is a three-level stacking model. The first two levels are xgboost and lightgbm, while the last level is simple weighted mean. All training and stacking are done with K-fold cross-validation to minimize information leakage. Feature engineering and parameter tuning are performed probabilistically through [Bayesian optimization](https://github.com/fmfn/BayesianOptimization/tree/master/bayes_opt).

You need to download these files from [Kaggle's website](https://www.kaggle.com/c/zillow-prize-1/data) and place them in the `/raw/` folder:

* `properties_2016.csv.zip`

* `properties_2017.csv.zip`

* `train_2016.csv.zip`

* `train_2017.csv.zip`

* `sample_submission.csv`