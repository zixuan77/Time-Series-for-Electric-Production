# Time-Series-for-Electric-Production

The industrial production (IP) index measures the real output of all relevant establishments located in
the United States, regardless of their ownership, but not those located in U.S. territories. The goal for this
project is to forecast the future data of industrial production (IP) index of electric and gas utility for the year
of 2009-2010 by appropriately modeling the time series data of electric and gas utility industrial production
(IP) index from 1985 to 2018.


This project includes the process of time series analysis which includes data transformation with Boxcox
and log transformation, model identification with acf and pacf plot, diagnostic checking with the analysis
of residuals and forecast. The plot of original data displays evident periodic pattern. Therefore, SARIMA
model is used to fit this electric production data set. Let the Y_t be the training data. $$ln(Y_t)$$ follows
$$SARIMA(2,1,2)(2,1,1)_12$$ model:$$(1 + 0.2440B^2 )(1 − 0.1771B^{24} )(1 − B)(1 − B^{12})ln(Y_t ) = (1 − 0.3960B −
0.5058B^2 )(1−0.7301B^12 )Z_t $$. The predicted data are close to the real(testing) data line, which indicates that
the model we choose fits well to the original data, but with little defect for the predicted confidence interval.
