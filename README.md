# Birth Rate Time Series Forecasting

## Summary of the Folder 

- `data` folder contains the data I used for the analysis 
- `plots` contains the plots generated 
- `notebooks` contains the key notebooks involved in analysis and consulting 
    - `birth-rate-forecasting.ipynb` is the notebook where I train the time series model to predict the birth rate 

## Methodology Used 

Instead of using traditional time series forecasting, I am using a ML driven framework and view of this problem. 

For birth rates, I obtained data from the National Population Statistics from a Thai website which I had to clean and reformat. 

I also then carried out data preprocessing and feature engineering by creating new and useful features like month, year and also lag features as well 

after preprocessing, I trained the model using XGBoost library and validating using time series cross validation. I also carried out hyperparameter fine-tuning using optuna to get the best parameters that lead to the best model performance. 

One of the limitation of XGBoost when using it to predict time series is that it may adapt too much to short-term fluctations instead of long term trends. so I used polynomial regression of degree 2 to fit to long-term trend first and then used XGBoost to fit the residuals. 

For my predictions, I simply re-added the residuals and the prediction from the polynomial 


