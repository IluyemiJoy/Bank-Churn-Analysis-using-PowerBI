# Bank-Churn-Analysis-using-PowerBI
A dynamic, interactive, multifaceted visualization tool built to explore bank customers churn- focusing on demographics, behaviors, and churn risk profile
---

<h2>1.	Project Overview</h2>

 <h3>•	Problem Statement</h3>

  The bank is experiencing an alarming trend: growing number of customers are closing their accounts and leaving. This project aims to **Uncover the secret patterns** behind customer churn by analyzing demographics, customer behaviour and interactions to answer th critical question: **“Why are customers ghosting our bank?”

  <h3>•	Objective:</h3>
  
  To uncover the secret patterns behind customer churn by digging into their demographics, behaviors, complaints, satisfaction scores, and product usage.

---

<h2>2.	Data Source</h2>

The data was obtained online from Kaggle

---

<h2>3.	Methodology</h2>

<h3>•	Tools Used</h3>
The dashboard was built using the following tools and technologies
-	**Power BI Desktop** – main data visualization platform used for report creation
-	**Power Query** – Data transformation and cleaning layer for reshaping and preparing data
-	**DAX (Data Analysis Expressions)** – Used for calculated measures
-	**Python in Power BI** – Tool for advanced analysis
-	**File format** - .pbix for development and .png for dashboards preview

<h3>•	Key Data Cleaning Processes</h3>

-	Credit score was recategorized into “Credit Score Range”, into Poor (<580), Fair (<670), Good (<740), Very good (<800) and Excellent (>=800)
-	Replaced 1 and 0s in “HasCrCard”, “IsActiveMember” to “Yes” and “No” respectively
-	Compilation of all cleaning processes

  
<h3>•	Key DAX Measures</h3>

**-	Churn rate** = DIVIDE([Churned], [Total Customers], 0)

**-	Avg Credit Churned** = CALCULATE(AVERAGE('Customer_Churn_Records'[CreditScore]),'Customer_Churn_Records'[Churn status] = "Churned"
-	Compilation of all DAX Measures

---

<h2>4.	Key Insights and Findings</h2>

This multifaceted dashboard provides a 360-degree view of the churn problem:

<h3>•	Demographic Analysis</h3>

[Dashboard Preview](https://github.com/IluyemiJoy/Bank-Churn-Analysis-using-PowerBI/blob/main/Demographic%20Analysis%20Dashboard%20Demo.PNG)

This tab analyzes the “who” – the geographic and demographic composition of customers
  -	Customers from Germany exhibit a significantly higher churn rate compared to other countries.
  -	Males across all age groups were identified as having a disproportionately higher churn rate
  -	Churning is significantly low across balances and almost equally distributed across all card types


<h3>•	Behavior & Engagement Analysis</h3>

[Dashboard Preview](https://github.com/IluyemiJoy/Bank-Churn-Analysis-using-PowerBI/blob/main/Behaviour%20and%20Engagement%20Analysis%20Dashboard%20Demo.PNG)

This tab explores the reasons for churning among customers
  -	Customers with a Basic product holding have marked a significantly higher churn rate
  -	Overall, a larger percentage of the customers have laid a complaint which in turn leads to an alarming churn in customers that have made complains 


<h3>•	Churn Risk Analysis</h3>

[Dashboard Preview]()
This tab profiles the customer churn risk
  -	The longer the customer stays the higher the tendency to churn
  -	Product holding and point earned have very weak hold on the churn rate

