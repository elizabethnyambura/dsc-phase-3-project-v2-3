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
















