# 05-04

---

## Project - Customer Churn

![](https://i.ytimg.com/vi/ON-iOsFK7co/maxresdefault.jpg)


## Objectives

Today, we will work on a new mini-project: we will build a **customer churn classifier** !

## Guidelines

The project is about a telecom company 🛰 : they want to **predict if a customer is about to leave**. We will combine both unsupervised and supervised approaches.

1. **Data preparation and EDA**. ⚠️ **Reminder**: Never dive too fast into modeling and predictions. In order to build great models, you first need to spend some time on data exploration, cleaning, visualization, feature engineering, etc.
2. **Market segmentation** : use clusterings models to determine meaningful clusters of customers and try to label them according to their main characteristics.
3. **Churn prediction** : use classifers and train them with the labeled dataset. Use the **F-score** to evaluate your model performance and aim for the best score 🏆. You can now use your clusters as features and try to identify which variables are the most important.  
4. [**Bonus question** : try to use [dataiku](https://www.dataiku.com/) to solve the same problem.]

➡️ Does any cluster rank as one of the most important variables in your predictions ?

> 

## Dataset

The dataset contains about **7000 customers** with **19 features**.

**Features** are the following:
- `customerID`: a unique ID for each customer
- `gender`: the gender of the customer
- `SeniorCitizen`: whether the customer is a senior (i.e. older than 65) or not
- `Partner`: whether the customer has a partner or not
- `Dependents`: whether the customer has people to take care of or not
- `tenure`: the number of months the customer has stayed
- `PhoneService`: whether the customer has a phone service or not
- `MultipleLines`: whether the customer has multiple telephonic lines or not
- `InternetService`: the kind of internet services the customer has (DSL, Fiber optic, no)
- `OnlineSecurity`: what online security the customer has (Yes, No, No internet service)
- `OnlineBackup`: whether the customer has online backup file system (Yes, No, No internet service)
- `DeviceProtection`: Whether the customer has device protection or not (Yes, No, No internet service)
- `TechSupport`: whether the customer has tech support or not (Yes, No, No internet service)
- `StreamingTV`: whether the customer has a streaming TV device (e.g. a TV box) or not (Yes, No, No internet service)
- `StreamingMovies`: whether the customer uses streaming movies (e.g. VOD) or not (Yes, No, No internet service)
- `Contract`: the contract term of the customer (Month-to-month, One year, Two year)
- `PaperlessBilling`: Whether the customer has electronic billing or not (Yes, No)
- `PaymentMethod`: payment method of the customer (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))
- `MonthlyCharges`: the amount charged to the customer monthly
- `TotalCharges`: the total amount the customer paid

And the **Target** :
- `Churn`: whether the customer left or not (Yes, No)

⚠️ As you can see, many features are **categorical** data with more than 2 values. You will have to handle this.