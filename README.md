# Telecommunication-Churn-Project
This dataset provides insights into customer churn in the telecommunications sector. It contains customer demographics, service usage, billing information, and churn status, making it useful for data analysis, visualization, and machine learning projects focused on customer retention.”



```sql
 SELECT *
FROM [Telecom data set];


SELECT COUNT(*) CustomerID 
FROM [Telecom data set];

SELECT churn,COUNT (*) AS Count 
FROM [Telecom data set]
GROUP BY Churn;

---Demographic Analysis---
SELECT gender, churn,COUNT(*) AS Count
FROM [Telecom data set]
GROUP BY gender,Churn;

SELECT SeniorCitizen, Churn,COUNT(*) AS Count
FROM [Telecom data set]
GROUP BY SeniorCitizen, Churn;

SELECT Dependents,COUNT(*) AS Count
FROM [Telecom data set]
GROUP BY Dependents;


----Tenure & Subscriptions Analysis 

SELECT Contract,Churn, COUNT(*) AS Count 
FROM [Telecom data set]
GROUP BY Contract,Churn;

---Avg tenure churned Vs Retained Cuestomers
SELECT Churn,AVG(Tenure) AS Avg_Tenure
FROM [Telecom data set]
GROUP BY Churn;
