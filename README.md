**PREDICTION OF SYRIATEL COMPANY CUSTOMER CHURN**


**BUSINESS UNDERSTANDING**

Due to increased competition in the telecommunication industry, there has been concerns on predicting the customer churn in order to retain customers. In order to maintain competitive parity by SyriaTel company, customer retention is a key to the business. Since retaining customers will be cheaper than acquiring new ones it is therefore paramount to deduce ways of making sure customers are not lost by the SyriaTel company. By analyzing various data points and using predictive analytics, SyriaTel company will identify patterns and indicators that help them anticipate customer behavior and take proactive measures to reduce churn rates. Therefore SyriaTel is seeking to models that will predict whether customers are likely to churn or not hence taking a proactive measures to retain them.data on demographics like location and usage patterns like calls, charge etc will be used to analyze and build predictive machine learning models, hence SeriaTel must continuously adapt its models to reflect changing customer behavior and market dynamics to ensure its retention strategies remain effective.

**OBJECTIVES**

* Create machine learning models that can predict customer churn by using data to analyze customer features.
* Comparing the build machine learning models and determine the most accurate model in prediction.
* The analysis aims to identify the specific features that have a significant impact on the customer churn rate in SyriaTel, provide valuable recommendations based 
  on the findings hence help to mitigate churn rates in the company and improve customer retention.

**DATA UNDERSTANDING**

  The project employs historical customer data, encompassing demographic details and transactional records from the Seriatel telecom company. This information is harnessed to construct a predictive model for categorizing customers into churned or non-churned groups. The dataset comprises 3,333 rows and 21 columns, and the company is headquartered in California, USA. The column titles are as follows:

* State: The state where the customer resides.

* Area code: The area code associated with the customer's phone number.

* International plan: A binary variable indicating whether the customer has an international calling plan (1) or not (0).

* Voice mail plan: A binary variable indicating whether the customer has a voicemail plan (1) or not (0).
  
* Number vmail messages: The number of voicemail messages the customer has.
  
* Total day minutes: The total number of minutes the customer used during the daytime.
  
* Total day calls: The total number of calls the customer made or received during the daytime.
  
* Total day charge: The total charges incurred by the customer for daytime usage.
  
* Total eve minutes: The total number of minutes the customer used during the evening.
  
* Total eve calls: The total number of calls the customer made or received during the evening.
  
* Total eve charge: The total charges incurred by the customer for evening usage.
  
* Total night minutes: The total number of minutes the customer used during the night.
  
* Total night calls: The total number of calls the customer made or received during the night.
  
* Total night charge: The total charges incurred by the customer for night usage.
  
* Total intl minutes: The total number of minutes the customer used for international calls.
  
* Total intl calls**: The total number of international calls the customer made.
  
* Total intl charge: The total charges incurred by the customer for international calls.
  
* Customer service calls: The number of customer service calls made by the customer.
  
* Churn: A binary variable indicating whether the customer has churned (1) or not (0).

* Total_calls: The total number of calls made or received by the customer across all periods (day, evening, and night).
  
* Total_charge: The total charges incurred by the customer across all usage periods.

**DATA PROCESSING**

We conducted a thorough examination to identify missing values, duplicates, as well as both categorical and numerical data, ensuring the cleanliness and proper formatting of the dataset for modeling. Additionally, we addressed class imbalances in the data and standardized it to establish consistency and uniformity for modeling purposes. This process was carried out to guarantee the validity, accuracy, and completeness of the data for modeling.

Furthermore, we performed the removal of outliers that could potentially distort the data and lead to inaccurate predictions. The chart below illustrates a box plot, showcasing the impact of the outlier exclusions.

![image](https://github.com/elizabethnyambura/dsc-phase-3-project-v2-3/assets/136367890/4e0615c7-b08b-4696-90d6-41e383d4143e)

**DATA ANALYSIS**

To gain deeper insights into our data, we created visualizations for various columns, exploring the relationships between churn rates, voice mail usage, international plan subscriptions, and the number of calls made within the United States.

![image](https://github.com/elizabethnyambura/dsc-phase-3-project-v2-3/assets/136367890/1de28741-2adc-4fd7-b9f6-302d65b0faee)

The above chart indicates that West (WV) state has the highest number of total calls while (CA) has the least number of total calls

![image](https://github.com/elizabethnyambura/dsc-phase-3-project-v2-3/assets/136367890/918c99b5-40d7-4a55-8c75-a0070a032db3)

The bar graph indicates that there is little variation among people making international calls concerning their choice of an international plan. On average, the number of international calls remains nearly consistent, regardless of whether individuals opt for an international plan or not.

![image](https://github.com/elizabethnyambura/dsc-phase-3-project-v2-3/assets/136367890/52746d16-9b27-4c30-80c9-dab19e1f3a3e)

The data on the chart reveals a significant correlation between the number of calls and loyalty.It suggests that a substantial portion of individuals who engage in these calls are loyal to Syriatel, resulting in a lower likelihood of them switching to another service provider.

![image](https://github.com/elizabethnyambura/dsc-phase-3-project-v2-3/assets/136367890/90add91f-3973-4380-ab9d-0b0a80671784)

The ghraphs above indicates that Voice Mail plan subscribers exhibit higher customer loyalty, primarily attributed to their lower churn rate. Conversely, customers who have subscribed to the international plan display a higher churn rate, indicating a greater probability of switching from Syriatel.

![image](https://github.com/elizabethnyambura/dsc-phase-3-project-v2-3/assets/136367890/cf2ee432-2329-4eb1-994b-471e99f5853e)

Graph features above exhibit a normal distribution, with the exception of customer service calls. Total international calls display a slight right skew, although it still maintains a relatively normal distribution.

Customer service calls, on the other hand, exhibit multiple peaks, indicating the presence of several modes within the population. This observation is logical since customer service calls are discrete integers and not continuous float numbers.

**MODELLING**


In our analysis, we constructed three models for predicting customer churn within the Seriatel company. These models are as follows:

Logistic Regression: Initially, it achieved an accuracy rate of 89.8% on the training data and 85.6% on the testing data. However, after implementing 5-fold cross-validation, the testing data accuracy improved to 84.8%, while the training data accuracy dropped slightly to 89.7%.

Decision Tree Classifier: This model initially attained an accuracy level of 88.6% on the training data and 91.1% on the testing data for predicting customer churn. Subsequently, after fine-tuning using grid search, the training accuracy improved to 91.7%, and the testing accuracy increased to 93.8%.

Random Forest Classifier: The initial accuracy of this model was 86.8% on the training data and 87.7% on the testing data. Following hyperparameter tuning, the accuracy on the training data substantially improved to 93.0%, with testing data accuracy reaching 91.0%.

After careful evaluation, we selected the two best-performing models, namely the Decision Tree and Random Forest, and further refined their hyperparameters using grid search. This optimization contributed to enhancing model performance and mitigating the risk of overfitting.

**EVALUATION**

Based on our analysis of the models, we have determined that the Decision Tree model is the most suitable choice for Seriatel in predicting customer churn due to its strong performance.

To further assess the model's performance, we generated ROC curves to evaluate the ROC accuracy and the area under the curve. We observed the following ROC scores for the three models: Logistic Regression (0.82), Decision Tree (0.91), and Random Forest Classifier (0.90).

After conducting hyperparameter tuning, we reaffirmed that the Decision Tree Classifier is indeed the superior model for predicting customer churn in Seriatel. The accuracy of this model improved following grid search tuning. While the Random Forest model is effective, it exhibits certain drawbacks, including increased complexity, longer execution times and overfitting tendencies after grid search tuning.

![image](https://github.com/elizabethnyambura/dsc-phase-3-project-v2-3/assets/136367890/e073dce3-ab41-482f-9d7b-60240a97435b)

**CONCLUSION**


The Decision Tree Classifier emerges as the optimal model for Seriatel's implementation.

This analysis equips Seriatel with the capability to:

* Achieve precise customer churn predictions.
* Realize cost savings through the formulation of effective customer retention strategies.
* Assure customer retention.
* Foster the development of robust business strategies and data-driven decision-making by gaining invaluable customer insights and understanding customer 
  behavior

**RECOMMENDATIONS**

* Continuous Model Optimization: Regularly fine-tune and optimize the decision tree model as new data becomes available.
  
* Benchmarking: Compare the performance of the decision tree model with industry benchmarks to gauge its effectiveness and competitiveness.

* Long-Term Strategy: Use the insights from the model to shape the company's long-term strategic direction
  
* Customer Feedback Analysis: Leverage the model's predictive capabilities to analyze and act upon customer feedback more effectively.

* Segmentation: Use the model's insights to segment the customer base into different groups based on churn risk and behavior

**NEXT STEPS**

* Regular Model Reevaluation: Periodically revisit the model's performance and consider retraining or updating it as necessary to adapt to changing market 
 dynamics.

* Customer Retention Strategies: Develop and execute customer retention strategies based on the insights and predictions provided by the model. 

* Training and Awareness: Educate and train relevant teams within the company on how to utilize the model's insights for better decision-making.

* Long-Term Strategy Development: Leverage the collected data and customer behavior insights to formulate long-term business strategies that align with customer 
  needs and market trends.































