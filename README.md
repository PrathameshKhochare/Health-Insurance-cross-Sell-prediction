# Health-Insurance-cross-Sell-prediction
This is a note book of cross selling of health insurance customers on vehicle insurance product and using machine learning to predict whether a customer is interested or not in vehicle insurance.

# Background Information :
An Insurance company that provide Health Insurance to its customers,the company wants to know if its customers from the previous year would also be interested in purchasing vehicle insurance from them.In this case we will build a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.

# Problem Statement:
* To improve the customer reach-out process, the insurance company wants to optimize its sales approach. Currently, many insurance workers spend a considerable amount of time meeting with prospective clients without any knowledge of the likelihood of the customer buying an insurance product. Therefore, the company wants to develop a model that can accurately predict the probability of a customer buying an insurance product, which would help the insurance workers to focus their efforts on the customers who are most likely to purchase a policy. This would ultimately save time and increase the efficiency of the sales process.

# Business Goals: 
* Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

# Workflow :
* Initial preparations(Loading the dependencies and the data)

1. Know Your Data
2. Understanding your Data
3. Data Wrangling
     * Handling null values
     * Handling duplicate values
     * Removing Outliers
     * Feature engineering
4. Data Vizualization, Storytelling & Experimenting with charts : Understand the relationships between variables
     * Univariate
     * Bivariate
     * Multivariate
5. Hypothesis Testing
6. Feature Engineering & Data Pre-processing
     * Handling Missing Values
     * Handling Outliers
     * Categorical Encoding
     * Feature Manipulation & Selection
     * Data Transformation
     * Data Splitting
     * Handling Imbalanced Dataset
         * SMOTE (Synthetic Minority Oversampling Technique)
     * Data Scaling
7. ML Model Implementation
     1. Logistic Regression
     2. Random forest
        * Cross- Validation & Hyperparameter Tuning
     3. Naive Bayes
     4. KNN
     5. SVM
        * Cross- Validation & Hyperparameter Tuning
     6. XGboost
        * Cross- Validation & Hyperparameter Tuning
* Model Result
* Model explainability
    * SHAP
8. Conclusion

<details>
<summary>Click to see the conclusion and recommendation</summary>
<br>

## Conclusion: 
Conclusions drawn from EDA  -:
1. From this dataset of health insurance, **Only 12 percent** of people are interested in Vehicle Insurance.
2. **Almost 96%**(53-> between 1-2 Year + 43 -> less than 1 Year) of customers have a vehicle age that's **less than 2 years.** from our analysis, customers who has more than 2 years of vehicle age are more interested with vehicle insurance advertisment, while customers who has **less then one year** of vehicle age, **only 4%** of them are actually interesred with vehicle insurance.
 * 17.3 % people with Vehicle age between 1 to 2 years are interested in Insurance.
 * 4.37 % people having vehicle age less than 1 year are interested in insurance.
 * 29.37 % people having vehicle age more than 2 years are interested in Insurance.
3. we also found out that a newer vehicle are more likely to have a vehicle insurance, with vehicle that's **less than one year 66% of those are insured** , vehicle that's **older than one year but less than 2 years are 33% insured**, while **less than one percent of vehicle that's older than 2 years are insured.** This should explain why customer who owns a newer vehicle are less likely to be intersted with insurance promotion, because they probably alredy have one. 
4. Almost every customer **who already have a vehicle insurance** is **not interested** with another vehicle insurance. **54%** people are not insured yet.out of all customer who does not have a vehicle insurance almost a **quarter(23%)** of them **are intersted** with vehicle insurance.
5. **Middle age** people are more interested in vehicle insurance **(20.04%)** as compared to Oldage(9.68%) and Youngage (6.55%).
6. **71% middle age** people are **not** previously insured. 63% Oldage and 37% Young age customers are not insured yet.
7. Customers **who never had vehicle damaged only 0.5 % of those customers are intersted** with vehicle insurance, 87% of customers who never had any vehicle damaged already have a vehicle insurance.
8. **99%** of Youngage have a vehicle that's **less than one year** of age, and from our analysis before that vehicle that's less than one year are 66% already insured. also almost 63% of Youngage people are already have vehicle insurance.
    
 **This conculed that Youngage are more likely to already have a vehicle insurance before our vehicle insurance team approached, and that's a major factor why Youngage are least likely to be interested with our vehicle insurance, because they already have one.**

**So who's actually interested with our vehicle insurance ?**
 
From the responses there are **12 % of our health insurance customers are interested** with the vehicle insurance product but who are those people?
    
1. **First, Customer who does not have a a vehicle insurance**, out of all customers who does not have a vehicle insurance **22.5 %** of them says that they're interested with vehicle insurance product

2. **customers who has vehicle that's older than 2 years** our analysis before mentioned that only less than **one percent** of car that's older than 2 years are previouly insured, by not having a vehicle insurance they're more likely to be intersted with our vehicle insurance, our data show's that customer who has vehicle that's more than 2 years are **7 times** more likely to be intersted with vehicle insurance compared to customer who own a vehicle less than one year.

3. **customers who have had a vehicle damaged in the past from our analysis we found out that **95 %** of customers who have had vehicle damage in the past still doesn't have a vehicle insurance.

**Which Customer Generation that's most likely to be interested in Vehicle insurance ?**
 
 our analysis shows that **Middle age** has the highest percentage to be intersteed with vehicle insurance, to be precise, **20.03 %** of GEN X are interested with vehicle insurance, this might be because **71% Middle age** people does not have a vehicle insurace, and Middle age has the highest percentage of vehicle damager the past **(67%)** among other generation.
