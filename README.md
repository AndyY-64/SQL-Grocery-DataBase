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
  1. Query #1 (Total Sales per Store)
    - Query 1
     What are the total sales for each individual store?
     This query calculates the sum of total sales for each individual store, and this helps managers analyze which stores are performing well or need improvement. 
     
  3. Query #2 (Products Below Reorder Level)
    - Query 2
     What items are low in stock?
     This query notifies the manager when certain items' stock is low, and that helps managers restock before they run out of an item.
     
  5. Query #3 (Top 5 Best Selling Products)
    - Query 3
     What items are top-selling in the company?
     This query identifies the top-selling products of the company, which allows managers to figure out what to promote and what to keep when cycling out inventory to maintain high sales.  
     
  7. Query #4 (Average Transaction Value)
    - Query 4
     What is the average amount a customer spends in the store?
This query summarizes how much the average customer spends in a store, which allows managers to analyze how much the average customer spends and how it contributes to the overall sales of the company. 
     
  9. Query #5 (Suppliers with Above Average Costs)
    - Query 5
     
  10. Query #6 (Stores That Have Never Sold a Certain Category)
    - Query 6
      
  11. Query #7 (Customers Who Spent More Than $500)
    - Query 7

  12. Query #8 (The 5 most recent Orders)
    - Query 8

  13. Query #9 (Customers with the Most Transactions)
    - Query 9

  14. Query #10 (Product Cost Above Average Price in Their Category) 
    - Query 10


DATABASE INFORMATION: 
Database Name: grocery_chain_db
Additonal Information:
  - Database created using MySQLWorkbench 8.0C
  - 
