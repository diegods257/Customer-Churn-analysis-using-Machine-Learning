# Customer Churn analysis using Machine Learning

### It has become an important task for companies to understand customer behavior, as this allows them to acquire new prospects. But since acquiring a customer is more difficult than retaining one, companies are looking for different ways to identify when a customer has a high probability of churn and implement retention measures to maintain their monthly revenue. The objective of this work is to explore the application of different machine learning models to predict churn-prone customers on a dataset from a communications company.

### Data set Characteristics
*   customerID: Customer ID
*   gender: Whether the customer is a male or a female
*   Senior Citizen: Whether the customer is a senior citizen or not (1, 0)
*   Partner: Whether the customer has a partner or not (Yes, No)
*   Dependents: Whether the customer has dependents or not (Yes, No)
*   tenure: Number of months the customer has stayed with the company
*   Phone Service: Whether the customer has a phone service or not (Yes, No)
*   Multiple Lines: Whether the customer has multiple lines or not (Yes, No, No phone service)
*   Internet Service: Customer’s internet service provider (DSL, Fiber optic, No)
*   Online Security: Whether the customer has online security or not (Yes, No, No internet service)
*   Online Backup: Whether the customer has online backup or not (Yes, No, No internet service)
*   Device Protection: Whether the customer has device protection or not (Yes, No, No internet service)
*   Tech Support: Whether the customer has tech support or not (Yes, No, No internet service)
*   StreamingTV: Whether the customer has streaming TV or not (Yes, No, No internet service)
*   Streaming: Whether the customer has streaming movies or not (Yes, No, No internet service)
*  Contract: The contract term of the customer (Month-to-month, One year, Two year)
*   Paperless Billing: Whether the customer has paperless billing or not (Yes, No)
*   Payment Method: The customer’s payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))
*   Monthly Charges: The amount charged to the customer monthly
*   Total Charges: The total amount charged to the customer
*   Churn Label: Whether the customer churned or not (Yes or No)  


The dataset was published by IBM and corresponds to customer churn or exit at a communications company. It consists of 7043 records with 21 characteristics each, of which 20 are the descriptor variables, such as gender, socioeconomic characteristics and the different services purchased with the brand, the last one is the target variable named "Churn".

### Download Link https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data

### The data were fitted using over-sampling and under-sampling techniques to balance them before entering them into the models, as well as assigning weights by classes using the unbalanced data. XGBBoost, Logistic Regression, Logistic Regression with PCA, Decission Tree and Random Forest models were implemented.


### For the proposed exercise, a high recall in class 1 (churn) is sought. Since the aim is to avoid false negatives, in other words, customers who are likely to cancel the service, but the model fails to detect them, having a high recall guarantees the effectiveness of the corporate measures applied for customer retention.

### The best training results were obtained with the XGBClassifier algorithm with a recall of 0.86 and an accuracy of 0.75, assigning weights and with unbalanced data.
