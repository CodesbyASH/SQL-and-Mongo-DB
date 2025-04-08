** SQL and Mongo-DB**
**
 Data Infrastructure Engineering (MySQL, Python & MongoDB)
**
This project showcases a comprehensive project developed as part of demonstrating real-world database engineering skills, involving SQL stored procedures, functions, triggers, Python scripting, and MongoDB integration.
This project's main goal was to integrate relational databases (MySQL), programmable data manipulation (Python), and NoSQL logging (MongoDB) in order to replicate a real-world data infrastructure system. It was created to demonstrate how several technologies may cooperate to effectively and securely store, update, and audit data.
---

 Project Highlights

🔹 SQL Tasks
Stored Procedures: 
  - `customer_representative`: Fetch customers by sales representative ID.
  - `product_description`: Join and fetch product and product line descriptions.
  - `highest_three`: Get top 3 product lines by average stock.

![image](https://github.com/user-attachments/assets/5ce8d0a6-d320-4739-9c10-a5a1ec5ccd2d)


 Functions:
  - `total_price`: Calculate the total price of a product based on quantity and price.
  - `total_price_range`: Use range filtering and aggregation logic.

![image](https://github.com/user-attachments/assets/0be3c8ab-48f1-46db-a620-297c215f8574)


Triggers:
  - `office_update_before`: Track updates to the `offices` table, logging old/new values with timestamp into a temp table `office_updates`.


🔹 Python Integration:
   Read & Update MySQL: A Python script that:
  - Prompts user input to update phone numbers in the `offices` table.
  - Commits changes dynamically using MySQL Connector.

    ![image](https://github.com/user-attachments/assets/4f487b1b-d7e2-45c8-a3fe-553940a7b60d)

![image](https://github.com/user-attachments/assets/01e2ab26-3a49-480f-90d0-7e5af649f2bd)


  MySQL to MongoDB Transfer:
  - Fetches data from `office_updates` table.
  - Inserts the audit trail into MongoDB’s `auditing.office_auditing` document collection.

![image](https://github.com/user-attachments/assets/ef992d34-02be-4c95-9416-f9ac9d89c6ad)

![image](https://github.com/user-attachments/assets/12f21d77-a833-4530-ae78-3b36d00dbbf3)

---

 Skills Demonstrated

MySQL:
  - Stored Procedures, Functions, Triggers, Temp Tables
  - Joins, Aggregations, Grouping, Filtering, Parameter Handling

Python:
  - Database connectivity with `mysql.connector`
  - User input handling and updates
  - Data migration to MongoDB with `pymongo`

MongoDB:
  - Document-based storage
  - Real-time audit logging using Python

---

 Real-World Value

This project simulates real-world applications like:
- Inventory and product management
- Sales tracking and performance metrics
- Change auditing and data governance
- Cross-platform data integration

---

 How to Run:

1. Ensure MySQL, Python, and MongoDB are installed and running.
2. Load SQL scripts to initialize tables, triggers, and functions.
3. Run Python scripts to interact with MySQL and MongoDB.



