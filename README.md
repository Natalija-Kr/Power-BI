# Power-BI

This project is a Power BI report that analyzes sales data from the AdventureWorks database. It's a sample database provided by Microsoft for learning and testing purposes. Specifically, the data contains information about sales, sales orders, products, sales territories, resellers and customers. The goal of this project is getting insights from various aspects of the sales data, including product sales performance, resellers’ performance and customers buying trends.

#### Below is model view:
![image](https://github.com/user-attachments/assets/a27a27e8-93e4-49c1-9b38-29b465593e9f)
 
#### In the project many various DAX formulas were used (some of them below):
1.	Total Sales = SUM('Sales'[Sales Amount])
2.	Total units sold = SUM(Sales[Order Quantity])
3.	Gross profit = [Total Sales]-[Total product cost]
4.	Total products sold = DISTINCTCOUNT('Sales'[ProductKey])
5.	Total product cost = SUM(Sales[Total Product Cost])
6.	Sales per product = DIVIDE([Total Sales],[Total products sold])
7.	Products in stock = COUNT('Product'[ProductKey])
8.	Increase Sales = [Total Sales]*Parameter_What_if[Parameter Value]+[Total Sales]
9.	Active sales = INT ( NOT ISEMPTY ( Sales) )

#### Below is an example of sales report:
![image](https://github.com/user-attachments/assets/b3352b60-883a-4518-888a-d655fc2428c8)

### This work is licensed by MIT license
