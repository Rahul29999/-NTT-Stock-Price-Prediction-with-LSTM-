# NTT-Stock-Price-Prediction-with-LSTM

                           Overview of the NTT stock price project
In this training, you will use NTT stock price data to build a time series data forecasting model. You will begin with exploratory data analysis (EDA) of the data, and ultimately evaluate the accuracy of the model. You will use machine learning to predict stock prices and verify their accuracy, aiming to apply it in practice.
# Task Content
1.	Read and analyze the Data
Summary :  make table of contents and Import libraries to Use NTT stock price data to check data statistics, detect trends and seasonality over time, and check for outliers.
Goal : Identify trends in data and extract answers for predictive modeling.
2.	Data Visualization
	overview:use seaborn  and matplot library to plot the Correlation Heatmap , historiogram plot 
  and Feature Distribution of columns   
3.	Data preprocessing and feature engineering.
Overview : Perform preprocessing such as missing value handling,  and scaling to create features that are useful for stock price prediction. Goal : Prepare data to improve model accuracy.
4.	Model Selection and Training
Overview :Using LSTM models for time series forecasting is advantageous because they are designed to handle sequential data, making them ideal for ordered time series. LSTMs effectively retain information over long periods, capturing long-term dependencies that are crucial in forecasting. They also mitigate the vanishing gradient problem often faced by traditional RNNs, allowing for better learning from extended sequences. LSTMs can manage variable-length input data and integrate additional influencing factors, such as exogenous variables, enhancing forecasting accuracy. Their high performance often surpasses traditional statistical methods, and they excel at modeling complex, non-linear relationships within the data. Overall, LSTMs are a powerful choice for time series forecasting due to these capabilities.
6.	Evaluating the model and analyzing the results
Overview :The evaluation of various models for time series forecasting reveals notable performance differences. The Random Forest model achieved the highest R² score at 37.78%, indicating it effectively captures some variance in the data, followed by CatBoost with 33.30%. In contrast, models like AdaBoost (-2.38%), K-Nearest Neighbors (-20.73%), and SGD Regressor (an extreme negative score) performed poorly, failing to provide meaningful predictions. Overall, while Random Forest and CatBoost show promise, further refinement and exploration of other approaches, such as LSTM, may be necessary to enhance forecasting accuracy..
7. Conclusion
Summary : The evaluation of various models revealed that CatBoost Accuracy emerged as the best performer with an accuracy of 70.34%, closely followed by Random Forest at 69.25% and Decision Tree at 66.21%. In contrast, K-Nearest Neighbors exhibited poor performance at 50.71%, while both AdaBoost and Support Vector Machine also demonstrated weak results, with accuracies of 55.12% and 52.16%, respectively.
Regarding regression analysis, Random Forest achieved the highest R² score of 37.78%, while several models, including AdaBoost (-2.38%) and K-Nearest Neighbors (-20.73%), displayed negative R² scores, indicating a poor fit for the data.
The LSTM model demonstrated a Root Mean Squared Error (RMSE) of 2.35.
Predicting a consistent decline in stock prices over the next 30 days, starting at 180.44 and gradually decreasing to 167.76. Overall, traditional models are effective for classification tasks, while the LSTM model shows promise for time series forecasting.
