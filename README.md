# SQL-Grocery-DataBase
UGA MIST 4610 Spring 2026 Group Project Repository 

TEAM MEMBERS:
1. Andrew Yancey, - https://github.com/AndyY-64
2. Kristina Lam, - https://github.com/sybiesuga
3. Bryan Yang, - https://github.com/BryanYangUGA
4. Shivani Menon, - https://github.com/shivanimenon 
5. Andrew Pruitt, - https://github.com/andrewpruitt033


PROBLEM DESCRIPTION:
Our mission is to build a relational database modeling a regional grocery store chain operating multiple locations across the southeastern United States. The primary entity in the model represents each stores unique "LocationID" - the specific location of each grocery across the southeast. Each store offers a variety of products grouped by category and sourced from a multitude of 3rd party suppliers. The database will support employee tracking, inventory management, customer transactions, and orders from suppliers. Using sample data, we will generate meaningful queries that will assist managers and executives in analyzing sales, tracking inventory, and managing store profitabiltiy. 

DATA MODEL:
The purpose of Project 1's data model was to assist a chain of supermarkets in effectively and efficiently managing its inventory, orders, customers, employees, suppliers, categories, and store locations. The model uses normalized relational tables with primary and foreign keys to describe real-world business relationships and preserve data integrity. While suppliers and categories can be connected to several items, each product in the data model is a member of a single category and is provided by a single supplier. The problem of clients submitting many orders, each handled by a single employee and including different products, is resolved by the Order Item table, which keeps track of quantity and unit price. An inventory table is used to track the many-to-many relationship between products and stores by tracking inventory across several store locations. The store locations are managed by employees, and all relationships are enforced using foreign keys.

DATA DICTIONARY:

QUERIES:
  1. Query #1 (Total Sales per Store)
    - Query 1 displays the total sales for each individual store
     
  2. Query #2 (Products Below Reorder Level)
    - Query 2
     
  3. Query #3 (Top 5 Best Selling Products)
    - Query 3
     
  4. Query #4 (Average Transaction Value)
    - Query 4
     
  5. Query #5 (Suppliers with Above Average Costs)
    - Query 5
     
  6. Query #6 (Stores That Have Never Sold a Certain Category)
    - Query 6
      
  7. Query #7 (Customers Who Spent More Than $500)
    - Query 7

  8. Query #8 (Employees Hired in Last Two Years)
    - Query 8

  9. Query #9 (Products Supplied by More Than One Supplier)
    - Query 9

  10. Query #10 (Product Cost Above Average Price in Their Category) 
    - Query 10


DATABASE INFORMATION: 
Database Name: grocery_chain_db
Additonal Information:
  - Database created using MySQLWorkbench 8.0C
  - 
