# Health-Insurance-cross-Sell-prediction
This is a note book of cross selling of health insurance customers on vehicle insurance product and using machine learning to predict whether a customer is interested or not in vehicle insurance.
![228839831-fb6d6085-eee8-46f9-abfa-223e564d5dae](https://user-images.githubusercontent.com/121234763/233061900-08233bb6-ad5b-45bf-b4d3-9b185a3058b0.png)

# Background Information :
An Insurance company that provide Health Insurance to its customers,the company wants to know if its customers from the previous year would also be interested in purchasing vehicle insurance from them.In this case we will build a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.
![228839831-fb6d6085-eee8-46f9-abfa-223e564d5dae](https://user-images.githubusercontent.com/121234763/233061921-61635004-cb22-4b5a-93ac-c967cbfbaa50.png)

# Problem Statement:
* To improve the customer reach-out process, the insurance company wants to optimize its sales approach. Currently, many insurance workers spend a considerable amount of time meeting with prospective clients without any knowledge of the likelihood of the customer buying an insurance product. Therefore, the company wants to develop a model that can accurately predict the probability of a customer buying an insurance product, which would help the insurance workers to focus their efforts on the customers who are most likely to purchase a policy. This would ultimately save time and increase the efficiency of the sales process.
![228839831-fb6d6085-eee8-46f9-abfa-223e564d5dae](https://user-images.githubusercontent.com/121234763/233061935-75467160-e094-4659-9427-e67f32cb6c9c.png)

# Dataset
The dataset is from Vehicle Insurance company. The data set includes over 381109 records and 12 attributes based on historical usage patterns.For more information on the dataset, please visit the Kaggle website at 
"https://www.kaggle.com/datasets/anmolkumar/health-insurance-cross-sell-prediction"
![228839831-fb6d6085-eee8-46f9-abfa-223e564d5dae](https://user-images.githubusercontent.com/121234763/233061942-0ac2289c-1cea-40ba-8215-dd413793e527.png)

# Dataset description:
* ID: Unique identifier for the Customer.
* Age: Age of the Customer.
* Gender: Gender of the Customer.
* Driving_License: 0 for customer not having DL, 1 for customer having DL.
* Region_Code: Unique code for the region of the customer.
* Previously_Insured: 0 for customer not having vehicle insurance, 1 for customer having vehicle insurance.
* Vehicle_Age: Age of the vehicle.
* Vehicle_Damage: Customer got his/her vehicle damaged in the past. 0 : Customer didn't get his/her vehicle damaged in the past.
* Annual_Premium: The amount customer needs to pay as premium in the year.
* Policy_Sales_Channel: Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.
* Vintage: Number of Days, Customer has been associated with the company.
* Response (Dependent Feature): 1 for Customer is interested, 0 for Customer is not interested.
![228839831-fb6d6085-eee8-46f9-abfa-223e564d5dae](https://user-images.githubusercontent.com/121234763/233061954-8cd76997-1939-45ff-b305-0adb29bb1839.png)

# Business Goals: 
* Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.
![228839831-fb6d6085-eee8-46f9-abfa-223e564d5dae](https://user-images.githubusercontent.com/121234763/233061964-e21a1b8e-e5b8-4dbd-a4c5-ef280cdae221.png)

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
![228839831-fb6d6085-eee8-46f9-abfa-223e564d5dae](https://user-images.githubusercontent.com/121234763/233061996-4be90f22-f04e-43e1-92f0-b66024e36d16.png)

<details>
<summary>Click to see the conclusion and recommendation</summary>
<br>

# Conclusion: 
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

    
Conclusions drawn from ML Model -:
* Implimented 6 classification ML Models Logistic Regression, Random forest, XGboost, Naive Bayes, KNN and SVM in our analysis.
* Considered Naive_bayes as our final optimal model as we are getting highest recall(96%), f1 score(81%), accuracy(78%) and auc-roc(84%) from it.
* Age, sex and pulse pressure are the** highest contributing features** towards the predictions.
![228839831-fb6d6085-eee8-46f9-abfa-223e564d5dae](https://user-images.githubusercontent.com/121234763/233062015-ba1e7f39-2d37-46bd-89ed-b97a2b6085ec.png)
 
    
# Recommendation

1. Work with dealership to capture millenial market
as we know from the analysis that millenials are less likely to be intersted with vehicle insurance because of most of them have a vehicle that's less than one year of age, and vehicle with less then one year of age are most likely to be insured so in conclution they already have one, and so they're not interested. By working together with a dealership that sells a brand new car, we could tackle this problem, our insurance company could have a bundling product of brand new vehicle and a free promotional vehicle insurance for certain period of months. we hope that by working together with vehicle dealership we could target more millenials customers.

2. Target & Educate Customers Who had Vehicle Damage in the past
95% customers who have had a vehicle damaged in the past still does not have a vehicle insurance this is a gold mine for our vehicle insurance, since customers are more likely to be interested in vehicle insurance if they've a vehicle damage in the past.

we could to a targeted marketing to this customers, by showing the benefits of having a vehicle insurance and how it will protect you if you ever had a vehicle damaged in the future

3. Benfits for customer who has a vehicle that's more than 2 years
having an older vehicle means having more problem compared to newer vehicle, problems like overheating, radiator problem and, etc are common with older cars, fixing those kind of stuff could be costly or having problem like that in the middle of a road could be troublesome. Since only less than one percent of customer who's actually owned car that's older than 2 years and insured, we could focus more on the problems that car over two years might have and the pain point of customers that owned older car and we should construct the benefits on those pain points, since customer with vehicle age over 2 years are the most likely to be intersted with vehicle insurance

4. Use Machine Learning Algorith to have predict the response outcome of a customer
Using the Logistic regression machine learning that has recall of 96.5 % will speed up and find out which customer who actually intersted in vehicle insurance, and we could focus our resource just based on the customers that's interested    
