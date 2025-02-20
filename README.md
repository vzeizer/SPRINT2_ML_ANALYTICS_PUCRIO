# SPRINT **Analytics – Descriptive and Predictive**. **MVP Project: Predicting Churn**

- **The Machine Learning problem to be tackled is a Time Series Classification to predict Customer Churn over time.**

**Churn rate**, also known as attrition rate, is a crucial metric used by businesses to measure the rate at which customers or subscribers discontinue their relationship with a service over a specific period of time. It is commonly expressed as a percentage and is calculated by dividing the number of customers lost during a given period by the total number of customers at the beginning of that period.

**Limitations and Considerations of Churn Rate:**

1. **Definition Consistency**: There may be variations in how churn is defined across different industries and companies. It's important to have a consistent definition of churn to ensure accurate and meaningful comparisons.

2. **Time Frame**: The choice of time frame for calculating churn can significantly impact the churn rate. Shorter time frames may result in more fluctuations, while longer time frames may obscure trends or changes in customer behavior.

3. **Customer Segmentation**: Not all customers are equal, and their behaviors may vary based on factors such as demographics, usage patterns, and tenure. Analyzing churn without considering these segments may overlook important insights.

4. **Customer Acquisition**: High churn rates can be offset by acquiring new customers. Therefore, it's essential to consider both churn and customer acquisition costs to evaluate the *overall health of a business*.

6. **Voluntary vs. Involuntary Churn**: Churn can be classified as voluntary (e.g., customers canceling subscriptions) or involuntary (e.g., customers moving away). **Understanding the reasons behind churn can help tailor retention strategies effectively.**

7. **Lagging Indicator**: **Churn rate is a lagging indicator, meaning it reflects past behavior rather than predicting future actions. To address this limitation, businesses may complement churn rate analysis with predictive modeling techniques to anticipate and prevent churn proactively.**

8. **Data Quality**: Churn rate calculations rely on accurate and reliable data. Poor data quality, such as incomplete or outdated customer records, can lead to inaccuracies in churn rate measurements.

9. **External Factors**: External factors beyond the company's control, such as market competition, regulatory changes, or economic conditions, can influence churn rates. These factors should be considered when interpreting churn rate trends.

In summary, while churn rate is a valuable metric for assessing customer retention and loyalty, it is essential to interpret it in context and consider its limitations and nuances to derive actionable insights effectively.


The following business goals and insights can be derived from this data and available features:

### Business Goals:
1. **Churn Prediction:**
   - The primary goal of the project could be to predict customer churn based on various features such as customer behavior, transaction history, and demographics.
   - By accurately predicting churn, the company can proactively take measures **to retain at-risk customers**, such as **offering personalized discounts**, improving customer service, or **introducing loyalty programs**.

2. **Customer Segmentation:**
   - **Utilizing features like sales_channel, segment_code, and group_code, the company can segment its customers based on their purchasing behavior, preferences, and demographics**.
   - This segmentation can help in targeted marketing strategies, product recommendations, and tailored communication to different customer segments.

3. **Seller Performance Analysis:**
   - Analyzing seller_code along with transaction data can help evaluate the **performance of individual sellers**.
   - Identifying top-performing sellers and areas for improvement can lead to **better sales strategies, training programs, and incentive structures for the sales team**.

4. **Optimizing Pricing Strategy:**
   - Analyzing unit_price and total_price data can provide insights into **pricing strategies and customer preferences**.
   - Understanding price elasticity and customer sensitivity to pricing changes can help optimize pricing strategies to **maximize revenue and customer satisfaction**.

### Insights and Lessons Learned:
1. **Identifying Key Drivers of Churn:**
   - Through feature importance analysis, the project can identify which factors contribute the most to customer churn.
   - Insights gained from the modeling process can highlight areas of improvement in customer service, product offerings, or overall customer experience.

2. **Understanding Customer Behavior:**
   - Analysis of transaction history and customer interactions can provide insights into customer behavior patterns, such as **purchase frequency, order size, and channel preferences**.
   - Understanding these patterns can help **tailor marketing campaigns, improve product offerings, and enhance customer engagement strategies**.

3. **Predictive Analytics for Future Growth:**
   - By building a predictive churn model, the company can forecast future churn rates and **anticipate potential revenue losses**.
   - These predictive insights can inform strategic decision-making and resource allocation to mitigate churn and drive business growth.

4. **Continuous Improvement and Adaptation:**
   - The project can serve as a foundation for ongoing monitoring, evaluation, and **refinement of business strategies**.
   - Continuous analysis of customer data and model performance can facilitate iterative improvements and **adaptation to changing market dynamics and customer preferences**.

Overall, the project aims to leverage data-driven insights to enhance customer retention, optimize sales strategies, and drive sustainable business growth in the face of evolving market challenges.

## **Business Problem Description: Churn Prediction in Retail Transactions**

**Background:**
In the retail industry, customer churn, or the loss of customers, can significantly impact a business's revenue and growth. Identifying and understanding the factors that contribute to churn is crucial for **developing targeted retention strategies**. In this context, **we aim to build a predictive model to identify customers at risk of churning based on various transaction-related features.**

**Objective:**
The primary objective is to predict customer churn in retail transactions. By leveraging historical transaction data, we intend to develop a model that can effectively **identify customers who are likely to discontinue their engagement with the business**. This predictive capability enables proactive retention efforts, allowing the company to **implement personalized strategies to retain valuable customers**.

**Data Overview**:
The dataset contains information related to customer transactions, encompassing a variety of features that capture different aspects of the customer's interaction with the retail platform. These features include customer identifiers, transaction details, item-related information, and indicators of the sales channel and seller involved. The target variable, **'is_churn,' denotes whether a customer has churned (1) or not (0)**.

**Features:**

1. customer_code: Unique identifier for each customer.

2. branch_id: Identifier for the branch associated with the transaction.

3. sales_channel: Channel through which the sale was made (e.g., online, in-store, etc.).

4. seller_code: Identifier for the seller involved in the transaction.

5. register_date: Date when the customer registered.

6. total_price: Total price of the transaction.

7. order_id: Identifier for the order associated with the transaction.

8. quantity: Number of items purchased in the transaction.

9. item_code: Identifier for the item purchased.

10. item_total_price: Total price of the item in the transaction.

11. unit_price: Price per unit of the item.

12. group_code: Code indicating the group/category to which the item belongs.

13. segment_code: Code indicating the segment to which the item belongs.

14. is_churn (Target): Binary variable indicating whether the customer churned (1) or not (0).

**Business Impact:**

**Proactive Retention Strategies**: Early identification of customers at risk of churning allows the implementation of **targeted retention strategies, such as personalized discounts, loyalty programs, or outreach campaigns.**

**Revenue Protection**: By reducing churn, the business can protect its revenue streams and **foster customer loyalty**, leading to sustained financial performance.

**Operational Efficiency**: Understanding the factors contributing to churn provides insights for operational improvements, **enhancing the overall customer experience and satisfaction.**

**Resource Optimization**: Targeting retention efforts based on predictive insights enables the **efficient allocation of resources, ensuring a focused approach to customers most likely to churn**.

**Success Metrics**:
The success of the churn prediction model will be evaluated based on metrics such as **accuracy, precision, recall, and the area under the ROC curve**. The business impact, measured by the effectiveness of implemented retention strategies and the reduction in churn rates, will also be key indicators of success.

**Next Steps**:

**Data Exploration and Preprocessing**: Conduct in-depth exploration of the dataset, handle missing values, and preprocess features as needed.

**Model Development**: Train and evaluate machine learning models, selecting the most suitable algorithm for churn prediction.

**Model Interpretability**: Use interpretability techniques, such as feature importance analysis, to understand the factors influencing predictions.

**Implementation and Monitoring**: Implement the predictive model in the operational environment and establish a monitoring system to track its performance over time (**future works**) .

The successful implementation of the churn prediction model will empower the business to take proactive measures, **strengthen customer relationships, and mitigate the impact of customer churn on its overall success.**


### Shortcomings (Restrictions), Limitations of the Data Analysis and respective Modeling

Some potential drawbacks, shortcomings, and limitations of the modeling and data analysis could include:

1. **Limited Feature Set:**
   - The dataset may lack certain key features that could significantly impact churn prediction and customer behavior analysis. For example, factors such as **customer demographics (age, gender, income), product reviews, customer service interactions**, or external factors like economic conditions and competitive landscape could provide valuable insights but are not included in the dataset.

2. **Data Quality Issues:**
   - The dataset may suffer from data quality issues such as missing values, **inconsistencies**, or errors, which can affect the accuracy and reliability of the modeling results.
   - **Incomplete or inaccurate data** may lead to biased predictions and unreliable insights.

3. **Imbalanced Class Distribution:**
   - The target variable 'is_churn' may exhibit class imbalance, with a significantly higher proportion of non-churn instances compared to churn instances.
   - **Imbalanced class distribution can bias the model towards the majority class and result in poor performance, particularly in terms of sensitivity to detecting churn instances**.

4. **Temporal Dynamics:**
   - The dataset may not adequately **capture temporal dynamics and seasonality** in customer behavior and churn patterns.
   - Churn prediction models may fail to generalize well to future time periods if the underlying patterns and relationships evolve over time.

5. **Limited Contextual Information:**
   - **The dataset lacks contextual information about customer interactions, preferences, and sentiments**, which could provide deeper insights into churn drivers and customer satisfaction.
   - Without context, the model may struggle to capture nuanced customer behaviors and accurately predict churn.

6. **Feature Engineering Challenges:**
   - The dataset may require additional feature engineering to extract meaningful insights and capture complex relationships between variables.
   - Manual feature engineering and domain expertise are crucial but may be limited by the availability of relevant data and the complexity of customer behavior.

7. **Model Interpretability and Explainability:**
   - Model interpretability is essential for gaining actionable insights and building trust with stakeholders.

These limitations requires careful consideration of data collection, feature selection, model development, and evaluation methodologies. Collaborative efforts between data scientists, domain experts, and business stakeholders are essential to mitigate risks and maximize the value of the modeling process.


## **Data Dictionary**

- The following shows the respective *Data Dictionary* for this dataset:

- customer_code:
Description: Unique identifier for each customer;

- branch_id:
Description: Identifier for the branch associated with the transaction;

sales_channel:
Description: Channel through which the sale was made (e.g., online, in-store, etc.);

- seller_code:
Description: Identifier for the seller involved in the transaction;

- register_date:
Description: Date when the customer registered;

- total_price:
Description: Total price of the transaction;

- order_id:
Description: Identifier for the order associated with the transaction;

- quantity:
Description: Number of items purchased in the transaction;

- item_code:
Description: Identifier for the item purchased;

- item_total_price:
Description: Total price of the item in the transaction;

- unit_price:
Description: Price per unit of the item;

- group_code:
Description: Code indicating the group/category to which the item belongs;

- segment_code:
Description: Code indicating the segment to which the item belongs;

- is_churn:
Description: Target variable indicating whether the customer churned (1) or not (0).


## **Some Questions to be Answered here:**

1. What are the most important factors/features that are responsible for customer churn? And for normal/not churned events?
2. Which are the segments more prone to churn outcomes?
3. Which are the groups more prone to churn outcomes?
4. Which are the sellers more prone to churn outcomes?
5. Which are the sellers that are the most relevant in order to take into account when using ML methods?
6. How is the distribution of events, churned or not churned? And the distribution throughout the years? Are there specific years that might be showing data drift?
7. Which is the best model to describe the data according to the Area Under the ROC Curve? Which are the most important features in the overall predictions of the dataset? Are lagged features relevant to best model this data?
8. What is the performance of the best model in the training and testing data? Has there been some degree of underfitting or overfitting?
9. There could have been used more advanced modeling of the data, such as ensemble and stacking? Is this model strategy worth it in this specific problem?  
10. How does the most relevant features contribute to churn or normal/not churned outcomes? Are lagged features of relevant impact in these specific prediction outcomes?


![logo](images/1_churnevents.png)


![logo](images/2_churnsegment.png)

![logo](images/3_churngroup.png)

![logo](images/4_churnyear_groupcode.png)

![logo](images/5_churnyear.png)

![logo](images/6_churnyear_scatter.png)

![logo](images/7_totalpricesegment.png)

![logo](images/8_totalprice_groupcode.png)

![logo](images/9_corrmatrix.png)

![logo](images/10_ML_randomCV.png)

![logo](images/10_ML_randomCV_timetaken.png)

![logo](images/12_ML_featimp.png)

![logo](images/13_cumsum_featimp.png)

![logo](images/14_precisionrecall_testset.png)

![logo](images/15_confusionmatrix.png)

![logo](images/15_confusionmatrix_testset.png)

![logo](images/17_featureimp_normalSHAP.png)

![logo](images/18_featureimp_churnSHAP.png)

![logo](images/19_violin_normalSHAP.png)

![logo](images/20_violin_churnSHAP.png)






























## **Conclusions and Discussion**

- **ANSWERING THE QUESTIONS ABOUT THE DATASET**:

1. What are the most important factors/features that are responsible for customer churn? And for normal/not churned events?

*Ans.:* For normal events, it was shown by SHAP analysis that the lagged features of "segment_code" are the most importante along with "group_code" related features. For churn events, it was observed by SHAP analysis that the lagged features of "segment_code" are the most importante along with "group_code" related features, however, in comparison to the former situation (normal outcomes), the "group_code" play a more significant role in these predictions.

2. Which are the segments more prone to churn outcomes?

*Ans.:*  **It was shown that segment numbers 2 and 3 have high churn rates.** So, it can be a good idea to take a careful at these segment in order to find policies to minimize churn.

3. Which are the groups more prone to churn outcomes?

*Ans.:* It was shown that **groups 1 and 2 have a very high churn rate**. Therefore, it might be interesting to take a careful look at these groups and use strategies to minimize churn especially for them.

4. Which are the sellers more prone to churn outcomes?

*Ans.:* It was shown that sales channels number **2, 4,7 and 9 have a churn rate much higher than not churned events**, so, special attention should be paid to these sales channels in order to minimize churn outcomes.

5. Which are the sellers that are the most relevant in order to take into account when using ML methods?

*Ans.:* As in the previous question, these are the sales channels number **2, 4,7 and 9 have the highest number of overall events**; we just kept for further analysis sales channels with **number of events greater than 200**.

6. How is the distribution of events, churned or not churned? And the distribution throughout the years? Are there specific years that might be showing data drift?

*Ans.:* In the dataset, approximately 80% are normal events, while 20% are churn events. It was shown that years 2016, 2017 and 2018 seem also to have a churn rate distribution different than the previous years. This is because that from 2008 up to 2015 the churn rate was augmenting quasi-linearly, and ,after these years, it is not anymore.

7. Which is the best model to describe the data according to the Area Under the ROC Curve? Which are the most important features in the overall predictions of the dataset? Are lagged features relevant to best model this data?

*Ans.:* **The best model was a Random Forest Model with Robust Scaler Normalization, showing an AUC close to 1.0 in the Validation Set and 0.82 in the Testing Set**. The Precision and Recall scores were also significantly lower in the Testing Set, even though, this is a good model concerning the complexity of the data. The main features responsible for the outcomes of the model were the **"group_code" and "segment_code"** lagged features according to the Feature Importances analysis of the Random Forest Classifier. This confirms the hypothesis that lagged features are really important when handling time series and justifies their creations prior to data modeling. Other models have been tested (not shown), such as Logistic Regression, Decision Trees and SVM's. However, either was the model's performance poor or it took too long to train without relevant results.

8. What is the performance of the best model in the training and testing data? Has there been some degree of underfitting or overfitting?

*Ans.:* The model had an AUC close to 1.0 in the Validation Set and 0.82 in the Testing Set. This somehow shows an overfitting of the model - the confusion matrices corrobotared it -, which can be explained by temporal data drift in the Testing Set (years 2016 and 2017 were in the testing set). Underfitting was not detected.

9. There could have been used more advanced modeling of the data, such as ensemble and stacking? Is this model strategy worth it in this specific problem?  

*Ans.:* **There could have been created more complex models from the algorithms used in the Pipeline by using Ensemble or stacking techniques. However, the gain in performance would be low in comparison to the complexity of this new model. Moreover, if one wants to augment the predictive power of the current model, one could have used more lagged features in the Feature Selection procedure to better fit and evaluate the model**;

10. How does the most relevant features contribute to churn or normal/not churned outcomes? Are lagged features of relevant impact in these specific prediction outcomes?

*Ans.:* It was shown by SHAP analysis that "segment_code" and its lagged features are most responsible for normal events, even though some of them have a slightly contribution to churn events. "group_code" and its lagged features have a small impact in the model and this contribution is towards normal events.
For churn events, the the top "group_code" lagged features tend to have a contribution more prone to churn events, while "segment_code" are more prone to do the opposite.



## **Future Works and Improvements**
- To improve this project, it is intended to:

1. deploy the model and create an user interface using streamlit;
2. use **automated machine learning** packages, such as h20 and Auto ML, to sweep over an wider range of models when modeling the dataset;
3. use **lagged features composed of the target variable** when modeling the data. This approach can be complex to tackle when evaluating the model in the testing set, because one has to predict churn events over specific time windows;
4. use other variants of TimeSeriesSplit methods to temporally cross-validate the model;
5. experiment a greater variety of models and a larget set of hyperparameters to tune the models. This can be done with Bayesian search in a smart and quicker way.



# Contributor Covenant Code of Conduct

## Our Pledge

We as members, contributors, and leaders pledge to make participation in our
community a harassment-free experience for everyone, regardless of age, body
size, visible or invisible disability, ethnicity, sex characteristics, gender
identity and expression, level of experience, education, socio-economic status,
nationality, personal appearance, race, caste, color, religion, or sexual
identity and orientation.

We pledge to act and interact in ways that contribute to an open, welcoming,
diverse, inclusive, and healthy community.

## Our Standards

Examples of behavior that contributes to a positive environment for our
community include:

* Demonstrating empathy and kindness toward other contributions that are not aligned with this Code of Conduct, and will communicate reasons for moderation decisions when appropriate.

## Scope

This Code of Conduct applies within all community spaces, and also applies when
an individual, or aggression toward or disparagement of classes of individuals.

**Consequence**: A permanent ban from any sort of public interaction within the
community.

## Attribution

This Code of Conduct is adapted from the [Contributor Covenant][homepage],
version 2.1, available at
[https://www.contributor-covenant.org/version/2/1/code_of_conduct.html][v2.1].

Community Impact Guidelines were inspired by
[Mozilla's code of conduct enforcement ladder][Mozilla CoC].

For answers to common questions about this code of conduct, see the FAQ at
[https://www.contributor-covenant.org/faq][FAQ]. Translations are available at
[https://www.contributor-covenant.org/translations][translations].

[homepage]: https://www.contributor-covenant.org
[v2.1]: https://www.contributor-covenant.org/version/2/1/code_of_conduct.html
[Mozilla CoC]: https://github.com/mozilla/diversity
[FAQ]: https://www.contributor-covenant.org/faq
[translations]: https://www.contributor-covenant.org/translations is officially representing the community in public spaces.
Examples of representing our community include using an official e-mail address,
posting via an official social media account, or acting as an appointed
representative at an online or offline event.

## Enforcement

Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported to the community leaders responsible for enforcement at
[INSERT CONTACT METHOD].
All complaints will be reviewed and investigated promptly and fairly.

All community leaders are obligated to respect the privacy and security of the
reporter of any incident.

## Enforcement Guidelines

Community leaders will follow these Community Impact Guidelines in determining
the consequences for any action they deem in violation of this Code of Conduct:

### 1. Correction

**Community Impact**: Use of inappropriate language or other behavior deemed
unprofessional or unwelcome in the community.

**Consequence**: A private, written warning from community leaders, providing
clarity around the nature of the violation and an explanation of why the
behavior was inappropriate. A public apology may be requested.

### 2. Warning

**Community Impact**: A violation through a single incident or series of
actions.

**Consequence**: A warning with consequences for continued behavior. No
interaction with the people involved, including unsolicited interaction with
those enforcing the Code of Conduct, for a specified period of time. This
includes avoiding interactions in community spaces as well as external channels
like social media. Violating these terms may lead to a temporary or permanent
ban.

### 3. Temporary Ban

**Community Impact**: A serious violation of community standards, including
sustained inappropriate behavior.

**Consequence**: A temporary ban from any sort of interaction or public
communication with the community for a specified period of time. No public or
private interaction with the people involved, including unsolicited interaction
with those enforcing the Code of Conduct, is allowed during this period.
Violating these terms may lead to a permanent ban.

### 4. Permanent Ban

**Community Impact**: Demonstrating a pattern of violation of community
standards, including sustained inappropriate behavior, harassment of an
individual people
* Being respectful of differing opinions, viewpoints, and experiences
* Giving and gracefully accepting constructive feedback
* Accepting responsibility and apologizing to those affected by our mistakes,
  and learning from the experience
* Focusing on what is best not just for us as individuals, but for the overall
  community

Examples of unacceptable behavior include:

* The use of sexualized language or imagery, and sexual attention or advances of
  any kind
* Trolling, insulting or derogatory comments, and personal or political attacks
* Public or private harassment
* Publishing others' private information, such as a physical or email address,
  without their explicit permission
* Other conduct which could reasonably be considered inappropriate in a
  professional setting

## Enforcement Responsibilities

Community leaders are responsible for clarifying and enforcing our standards of
acceptable behavior and will take appropriate and fair corrective action in
response to any behavior that they deem inappropriate, threatening, offensive,
or harmful.

Community leaders have the right and responsibility to remove, edit, or reject
comments, commits, code, wiki edits, issues, and other