# Customer Churn Prediction and Analysis

## Project overview 

Telecommunication cooperation provides a dataset for its customers, offering a wide range of services, including phone lines, internet types, contract types, and internet connections.
The goal is to analyze and predict customer behavior, identify factors contributing to customer churn, and provide recommendations to improve retention.

Insights and recommendations are provided on the following key areas: 

  - Churn Behavior Analysis: Evaluation of churn patterns based on contract type, payment method, internet service, and additional features such as online security and device protection.

  - Customer Segmentation: Identification of key customer segments more likely to churn.
    
  - Service Usage Impact: Analysis of how services like streaming, online backup, and unlimited data influence customer loyalty and churn rate.
  
  - Demographic Trends: Analysis of customer churn based on demographic factors, including age, marital status, and state.

  - Recommendations: Strategic suggestions are provided to improve customer retention.

### 📊 Interactive Dashboard

  - An interactive Power BI dashboard is available for download [**here**](https://github.com/Mo7amed-tal3at/telecom-customer-churn-analysis-da/blob/main/Churn%20Analysis%20Dashboard.pbix).

### 🛠️ SQL Queries

  - The SQL queries used for data exploration and quality checks can be found [**here**](https://github.com/Mo7amed-tal3at/telecom-customer-churn-analysis-da/blob/main/Churn_data_queries.sql).

### 🤖 Prediction Model

  - The machine learning implementation for churn prediction can be accessed [**here**](https://github.com/Mo7amed-tal3at/telecom-customer-churn-analysis-da/blob/main/MLModel.ipynb).
 


## Data Structure 
  -  Below is an image that shows the structure of the data and the relation among entities
    -  ![image](https://github.com/user-attachments/assets/f115c977-527f-4ce7-91ce-fe24931b63d9)

## Executive Summary

### Overview of findings
   

- The **Kashmir** region has the highest churn rate at **57%**, indicating a critical area for customer retention efforts.
- Customers subscribed to **Fiber Optic internet** are more likely to churn compared to those using Cable internet.
- A significant portion of customers churn due to **better services offered by competitors**.
- Churn was significantly higher among customers subscribed to **Phone Services**, **Internet Services**, **Papperless Billing**, and those with **Unlimited Data** plans. This suggests that core service experiences may play a major role in customer decisions to leave.
- The **attitude of support personnel** was identified as the **second most common reason** for customer churn, highlighting the importance of customer service quality in customer retention.
- A machine learning model predicted that **376 customers are likely to churn**, with the majority located in **Uttar Pradesh**, **Maharashtra**, **Tamil Nadu**, and **Karnataka**. Most of these high-risk customers use **Credit Card** and **Bank Withdrawal** as their payment methods.

  
Below is the **Overview Page** from PowerBI dashboard. The entire interactive dashboard can be downloaded [here](https://github.com/Mo7amed-tal3at/telecom-customer-churn-analysis-da/blob/main/Churn%20Analysis%20Dashboard.pbix)

  - ![image](https://github.com/user-attachments/assets/024ffa59-d207-4cde-b4c6-73edac5abe56)


## 🔎 Deep Dive – Insights and Interpretation

This section presents a detailed breakdown of the key insights extracted from the dataset, along with interpretations that explain customer churn behavior and its potential causes.

### Churn by Region
- **Kashmir** recorded the highest churn rate at **57%**, significantly higher than other regions.
- This suggests potential issues in regional service quality, pricing, or competitor presence in that area.

### Internet Type & Churn
- Customers using **Fiber Optic** internet were more likely to churn compared to those on Cable.
- Fiber users may be more tech-savvy and sensitive to performance issues or competitor offerings.

### Payment Method & Churn
- The churn rate for users paying via **Mailed Check** was **37%**, while **Credit Card** users showed the lowest churn at **14%**.
- Traditional payment methods may be correlated with older or less-engaged customers, or may reflect outdated billing experiences.

### Unlimited Data & Churn
- Surprisingly, churn was high among customers with **Unlimited Data** plans.
- This may indicate dissatisfaction with network speed, throttling, or perceived unfair pricing despite “unlimited” offers.

### Reason for Leaving
- The most common reason for churn was **"Competitor had better devices/services"**, followed closely by **"Attitude of support person"**.
- This highlights the importance of both competitive offerings and high-quality customer service.

### Demographic Factors
- Older customers and unmarried individuals showed slightly higher churn tendencies.
- These groups may struggle with paperless billing or be more price-sensitive or responsive to promotions and competitor incentives.
  
## 💳 Payment Method & Paperless Billing
  - Customers who used credit cards or digital payment methods had lower churn rates, suggesting that convenient payment options help with customer retention.
  - However, Paperless Billing users had a surprisingly high churn rate — around 80% of them left the service.
  - This may be explained by the fact that a large portion of the customer base opting for paperless billing were over the age of 50, a group that might prefer traditional paper billing or find digital communication less accessible.
    
  - ### *interpretation*: The conflict between digital convenience and customer preferences highlights the need for personalized billing strategies that match the demographic profile of each segment.

### 🤖 Churn Prediction Model

To enhance the analysis, a machine learning classification model was developed to predict which customers are most likely to churn.

- The data was preprocessed by encoding categorical variables, handling missing values, and scaling numerical features.
- A Random Forest model was trained on the cleaned dataset.

🧠 **Prediction Outcome:**
- The model predicted **376 customers are likely to churn**.
- Most of these high-risk customers are located in:
  - **Uttar Pradesh**
  - **Maharashtra**
  - **Tamil Nadu**
  - **Karnataka**

- The majority of them use **Credit Card** and **Bank Withdrawal** as their payment methods.

✅ These predictions can help the company take proactive steps to retain valuable customers before they leave, by targeting them with personalized offers, surveys, or improved service.

---

### 💡 Summary of Key Drivers of Churn:
| Factor                | Effect on Churn |
|----------------------|-----------------|
| Fiber Optic Internet | ↑ Increased     |
| Month-to-Month Contracts | ↑ Increased |
| Mailed Check Payment | ↑ Increased     |
| Lack of Add-on Services | ↑ Increased  |
| Good Customer Support | ↓ Decreased     |
| Long-Term Contracts  | ↓ Decreased     |

---

## ✅ Recommendations (from insights):

Based on the analysis, the following recommendations are proposed to help reduce customer churn and improve retention:

1. **Focus on High-Churn Regions**  
   - Prioritize customer support, service quality, and promotional efforts in regions like **Kashmir**, where churn rates are the highest.

2. **Improve Fiber Optic Internet Services**  
   - Address performance or reliability concerns and consider bundling fiber with premium support or discounts to improve satisfaction.

3. **Promote Digital Payment Methods**  
   - Encourage customers to use **Credit Card** or **Auto-Pay** by offering incentives, while simplifying the transition from traditional methods like mailed checks.

4. **Reassess Paperless Billing Strategy**  
   - Offer physical billing options or onboarding support for customers aged 50+, who may struggle with digital systems and contribute to high churn in this group.

5. **Enhance Customer Support Quality**  
   - Provide soft-skills training for support staff and actively monitor support satisfaction, as poor support attitudes are a leading churn driver.

6. **Offer Retention-Friendly Contracts**  
   - Shift focus from month-to-month contracts to longer-term plans with added benefits, which are correlated with lower churn.

7. **Benchmark Against Competitors**  
   - Investigate why customers perceive competitor services or devices as better, and address these gaps through service improvements or updated offerings.
     
8. **Act on Predicted High-Risk Customers**
   - The machine learning model identified **376 customers** who are likely to churn. Most of them are located in **Uttar Pradesh**, **Maharashtra**, **Tamil Nadu**, and **Karnataka**, and use **Credit Card** or **Bank Withdrawal** payment methods.  
   - These customers should be **proactively targeted** with:
     - Personalized offers or loyalty rewards  
     - Feedback forms or satisfaction surveys  
     - Dedicated support follow-ups  

   Engaging with these users before churn happens can significantly improve retention and reduce revenue loss.
