# SQL-Grocery-DataBase
UGA MIST 4610 Spring 2026 Group Project Repository 

TEAM MEMBERS:
1. Andrew Yancey, - https://github.com/AndyY-64
2. Kristina Lam, - https://github.com/sybiesuga
3. Bryan Yang, - https://github.com/BryanYangUGA
4. Shivani Menon, - https://github.com/shivanimenon 
5. Andrew Pruitt, - https://github.com/andrewpruitt033


Lakhiwhal Suggestions: He said watch for the accidental many to many between employee and customer right 
And switch category to sections

PROBLEM DESCRIPTION:
Our mission is to build a relational database modeling a regional grocery store chain operating multiple locations across the southeastern United States. The primary entity in the model represents each stores unique "LocationID" - the specific location of each grocery across the southeast. Each store offers a variety of products grouped by category and sourced from a multitude of 3rd party suppliers. The database will support employee tracking, inventory management, customer transactions, and orders from suppliers. Using sample data, we will generate meaningful queries that will assist managers and executives in analyzing sales, tracking inventory, and managing store profitabiltiy. 

DATA MODEL:
The purpose of Project 1's data model was to assist a chain of supermarkets in effectively and efficiently managing its inventory, orders, customers, employees, suppliers, categories, and store locations. The model uses normalized relational tables with primary and foreign keys to describe real-world business relationships and preserve data integrity. While suppliers and categories can be connected to several items, each product in the data model is a member of a single category and is provided by a single supplier. The problem of clients submitting many orders, each handled by a single employee and including different products, is resolved by the Order Item table, which keeps track of quantity and unit price. An inventory table is used to track the many-to-many relationship between products and stores by tracking inventory across several store locations. The store locations are managed by employees, and all relationships are enforced using foreign keys.

DATA DICTIONARY:

<img width="664" height="289" alt="Screenshot 2026-03-28 at 12 01 13 PM" src="https://github.com/user-attachments/assets/04164bbd-a64c-4f1c-a668-bdda6af93027" />


QUERIES:

Query #1 (Total Sales per Store)
     What are the total sales for each individual store?
     This query calculates the sum of total sales for each individual store, and this helps managers analyze which stores are performing well or need improvement. 

   <img width="818" height="525" alt="Screenshot 2026-03-28 at 12 04 31 PM" src="https://github.com/user-attachments/assets/d456577c-ff2c-416f-893c-af52dacce7e1" />
  
Query #2 (Products Below Reorder Level)
     What items are low in stock?
     This query notifies the manager when certain items' stock is low, and that helps managers restock before they run out of an item.

<img width="818" height="525" alt="Screenshot 2026-03-28 at 12 07 15 PM" src="https://github.com/user-attachments/assets/6ee42a74-d548-4169-bbe0-91e50eee6e98" />

Query #3 (Top 5 Best Selling Products)
     What items are top-selling in the company?
     This query identifies the top-selling products of the company, which allows managers to figure out what to promote and what to keep when cycling out inventory to maintain high sales.  
     
<img width="814" height="520" alt="Screenshot 2026-03-28 at 12 09 34 PM" src="https://github.com/user-attachments/assets/21540657-e8b1-4f21-8582-ac5c6b9d85ac" />

Query #4 (Average Transaction Value)
     What is the average amount a customer spends in the store?
This query summarizes how much the average customer spends in a store, which allows managers to analyze how much the average customer spends and how it contributes to the overall sales of the company. 

<img width="815" height="516" alt="Screenshot 2026-03-28 at 12 10 30 PM" src="https://github.com/user-attachments/assets/2ea6c2f3-a4d0-42fb-9058-0eabe66787b7" />

Query #5 (Suppliers with Above Average Costs)
     What suppliers have higher than average prices? The query identifies suppliers whose average price is above the mean price of all products. This helps managers to look at supplier cost and see if any replacement in supplier is needed
  <img width="815" height="512" alt="Screenshot 2026-03-28 at 12 11 09 PM" src="https://github.com/user-attachments/assets/6917dc86-4813-42b4-9251-5bccea96ab86" />
  
Query #6 (Stores That Have Never Sold a Certain Category)
     This query can check which stores have not sold product from a certain section. It helps manager detect gaps in customer preference in different locations. Then each store can have their own items and matches the customers interest. 
 
 <img width="814" height="509" alt="Screenshot 2026-03-28 at 12 13 07 PM" src="https://github.com/user-attachments/assets/d5165194-9454-43e6-86d9-2f6018fd1379" />
  
Query #7 (Customers Who Spent More Than $500)
     This query identifies customers who spend more than 500 dollars. This helps managers to recognize high value customers and possibly have them become loyal customers by offering promotions, discounts and loyalty programs.

<img width="814" height="520" alt="Screenshot 2026-03-28 at 12 13 49 PM" src="https://github.com/user-attachments/assets/38831165-0516-4c9c-b8f5-38e994bad902" />

Query #8 (The 5 most recent Orders)
     What are the most recent orders made in the system? This query can track the latest orders based on the order date limited to the five recent transactions. This can help managers quickly and efficiently review sales activity and track performance.

<img width="816" height="515" alt="Screenshot 2026-03-28 at 12 14 18 PM" src="https://github.com/user-attachments/assets/dd6f05da-2b83-4b7b-a4a7-e28532fa7d6a" />

Query #9 (Customers with the Most Transactions) 
What customers have made the most transactions?
This query calculates the total number of transactions made by each customer by counting their orders, helping managers identify the most active or valuable customers.

<img width="813" height="516" alt="Screenshot 2026-03-28 at 12 14 52 PM" src="https://github.com/user-attachments/assets/24254594-b7c8-41a2-b0bf-70b296715bd2" />

Query #10 (Product Cost Above Average Price in Their Category) 
Which products are priced above the average price within their category?
This query identifies products whose prices are higher than the average price in their section, helping managers evaluate pricing strategies and identify premium or overpriced items.

<img width="812" height="505" alt="Screenshot 2026-03-28 at 12 15 36 PM" src="https://github.com/user-attachments/assets/aedbd0e4-eb50-49b5-aa5d-71d426f1f252" />

DATABASE INFORMATION: 
Database Name: al_Group_21482_G1
Additonal Information:
  - Database created using MySQLWorkbench 8.0C
  - Each query listed above is a store procedure which can be called using: CALL TP_Q#();
