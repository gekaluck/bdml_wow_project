# Seoul Bike Sharing Demand Prediction

## Summary
My final project within Big Data Machine Learning course.
The goal was to predict the number of Seoul bikeshare bikes to be used based on the day of the year, hour of the day and weather conditions information.
Utilization of such a model could enable better bike sharing demand fulfillment, which leads to higher customer satisfaction and revenue increase, while creating cost-cutting opportunities.

I have performed explorational data analysis, initiated regression models, performed cross-validation, grid search for parameter tuning and assessed results.

## Dataset
Seoul Bike Sharing Dataset weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.
Dataset: https://archive.ics.uci.edu/ml/datasets/Seoul+Bike+Sharing+Demand

## Algorithms X-validation performance assessment on training data
![image](https://user-images.githubusercontent.com/26655645/160290739-dfec10da-0673-461b-a0d2-837575e9b45e.png)

## LightGBM performance on testing data

![image](https://user-images.githubusercontent.com/26655645/160290787-4138dea1-bf50-4c89-85cb-df1891b9c6f9.png)

## Prediction assessment
![image](https://user-images.githubusercontent.com/26655645/160290809-6fb7a9a9-d096-4619-b1ec-3be388666f98.png)

![image](https://user-images.githubusercontent.com/26655645/160290813-41e70d78-f781-4093-9f0f-ad9e48675f5c.png)

## Conclusion

- The model developed with LigthGBM algorithm and thorough data preprocessing has shown solid performance beating headless AI (h2o.ai)

- Except for some days/hours with unusual demand, the model prediction on test data yields low relative error

- MEA is 84, while target variable values range from 3 to 3365, which I consider a decent performance

- Model can be used to predict bike sharing demand in Seoul; however, I assume extrapolation is not appropriate and a new model should be built to predict bike sharing demand in other cities, since context is crucial.

- Even though it would probably not be appropriate to use this model in other settings, the project has shown all steps necessary to recreate such a model in case the analogous data is available

- I expect significant increase in performance after training on 2-3 additional years of observations

