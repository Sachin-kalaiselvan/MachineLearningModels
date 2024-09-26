                                                      ****Airline Passenger Satisfaction Prediction****
                                                      

****Overview****
This project focuses on predicting airline passenger satisfaction based on a wide variety of factors related to their flight experience. The primary objective is to build and train machine learning models that can accurately classify whether a passenger was satisfied or dissatisfied. This predictive model could assist airlines in enhancing service quality by identifying key areas that influence customer satisfaction.

****Problem Statement****
Airlines collect a vast amount of data from their passengers, ranging from personal details to satisfaction scores for various services. This project tackles the problem as a binary classification task where the goal is to predict whether a customer was satisfied or not. The dataset includes multiple features such as inflight Wi-Fi service, ease of online booking, seat comfort, and flight delays.

****Dataset****
The dataset consists of airline passenger satisfaction surveys with 103,904 rows and 25 features. Key variables include:
Gender: Male/Female
Customer Type: Loyal/Disloyal customers
Type of Travel: Business or Personal travel
Flight Distance
Various satisfaction ratings: Inflight Wi-Fi service, Food and drink, Seat comfort, Online boarding, etc.
Departure and Arrival Delays (in minutes)
The dataset is well-suited for classification tasks and provides comprehensive insights into different factors affecting passenger satisfaction.

****Methodology****
The project follows a typical data science workflow:
**1. Data Preprocessing:**
Handling missing values and outliers.
Encoding categorical variables using One-Hot Encoding.
Scaling and transforming numerical variables to address skewness.

**2. Exploratory Data Analysis (EDA):**
Investigated the distribution of satisfaction across different variables.
Generated visual insights using pie charts, histograms, and box plots to understand the relationships between features and customer satisfaction.

**3. Modeling:**
Trained several classification models, including:
Logistic Regression
Decision Tree
Random Forest
AdaBoost
Gradient Boosting
XGBoost
Used GridSearchCV for hyperparameter tuning to optimize model performance.

**4. Feature Selection:**
Used Sequential Feature Selector to identify the most significant features affecting satisfaction, such as Inflight Wi-Fi service, Online Boarding, and Seat Comfort.

**5. Evaluation:**
Models were evaluated using accuracy, ROC-AUC, and F1 score.
The final model, XGBoost, achieved an accuracy of 96%, making it the best-performing model.

****Key Features and Insights****

**Most impactful features:**
* Inflight Wi-Fi service, Online Boarding, and Business Class travel were found to significantly affect customer satisfaction.
* Passengers in Business Class and those who traveled long distances were generally more satisfied.
* Passengers in Economy Class reported lower satisfaction levels, especially with services like food, seat comfort, and legroom.
**Model Performance:**
* The XGBoost model performed best with a 96% accuracy and high ROC-AUC scores, closely followed by the Random Forest model.
* Random Forest provided a good balance of accuracy and training time, but XGBoost outperformed it in handling complex data patterns.

****Conclusion****
The final XGBoost model provides accurate predictions for passenger satisfaction and offers actionable insights for airlines to enhance service quality. By focusing on key factors such as seat comfort, inflight Wi-Fi, and online boarding, airlines can improve customer satisfaction, particularly in Economy Class.

****Future Work****
* Future improvements could include:
* Analyzing deeper features such as weather conditions and seating arrangements.
* Incorporating external factors such as flight pricing and comparison with competing airlines.
* Improving model interpretability through SHAP or LIME to better understand how each feature contributes to the final prediction.
