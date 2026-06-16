USE sales_dashboard;

SELECT SUM(Amount) AS Total_Sales
FROM `sales dataset`;

SELECT SUM(Profit) AS Total_Profit
FROM `sales dataset`;

SELECT SUM(Quantity) AS Total_Quantity
FROM `sales dataset`;

SELECT Category, SUM(Amount) AS Sales
FROM `sales dataset`
GROUP BY Category;

SELECT State, SUM(Amount) AS Total_Sales
FROM `sales dataset`
GROUP BY State
ORDER BY Total_Sales DESC;

SELECT CustomerName, SUM(Amount) AS Total_Sales
FROM `sales dataset`
GROUP BY CustomerName
ORDER BY Total_Sales DESC
LIMIT 10;

SELECT `Year-Month`, SUM(Amount) AS Total_Sales
FROM `sales dataset`
GROUP BY `Year-Month`
ORDER BY `Year-Month`;