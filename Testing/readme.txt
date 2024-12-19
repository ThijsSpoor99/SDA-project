This folder tests Hypothesis 1, 2, and 3. Its results can be found in the Testing_figures folder.

H0: Vector Autoregression does not improve the Linear Regression Model in weather prediction. (Hypothesis_1.ipynb), (Hypothesis_1_DM_results)
Test: Diebold-Mariano test
Fail to reject: pressure, temp_mean, and temp_min
Reject: humidity, sunshine, global_radiation

H0: Seasonality does not make a variable more predictable in the VAR framework (in terms of lower RMSE). (Hypothesis_2.ipynb), (H2_trainings, H2_boxplots)
Test: Welsch’s Two Sample t-test
Fail to reject: Non-seasonality grouped VAR systems had lower RMSE values than seasonality grouped VAR systems. 

H0: Increasing the sample size does not have an effect on the predicting power of a Vector Autoregression. (Hypothesis_3.ipynb), (H3_DM_Test_Heatmap)
Test: Diebold-Mariano test
Reject: Humidity, Pressure, Global Radiation
Fail to Reject: Temp_mean, Temp_min, Temp_max
