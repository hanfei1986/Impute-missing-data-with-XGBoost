# Impute-missing-data-with-XGBoost
When signaficant amount of data in highly-important features are missing, what can we do? Impute the missing data with mean or median? In this Juyter notebook, I demonstrate embedding a XGBoost model to do the data imputation in the data transformer.

In this dataset, a lot of "cost" data missing, but they are quite important to predict "price".

![image](https://github.com/hanfei1986/XGBoost-missing-data-imputer/assets/59255164/0e6c7106-af83-4cad-850c-40541113952b)

If we impute the missing "cost" with its mean or median, there will be a spike in the imputed dataset. In contrast, imputing the missing "cost" with a XGBoost regressor which is embedded in the data transformer and predicts "cost" from other features is very effective.

![image](https://github.com/hanfei1986/Impute-missing-data-with-XGBoost/assets/59255164/4dd8f72c-3377-4524-8c4f-cb3a69913970)


