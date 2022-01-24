# Load_Predictor-XGBoost

Data_Aggregator: Weather Data (hourly) is downloaded from Government of Canada website (https://climate.weather.gc.ca/) using a bash script (as the hourly data is not aggegated and should be downloaded for each day individually) and the downloaded data is then aggregated along with the power consumption data downloaded from NS Power (https://www.nspower.ca/oasis/monthly-reports/hourly-total-net-nova-scotia-load), using this Python script.

Data_preprocess: As XGBoot algorithm requires parameters to be either in Int/Float/Boolean or as categorical values, we use this Python script to pre-process the aggregated data to make it ready to be ingested by XGBoost predictor.

XGBPredictor: This Script uses XGBoost algorithm to predict the power consumption of the NS province.
