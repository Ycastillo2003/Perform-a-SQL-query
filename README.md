![image](https://github.com/user-attachments/assets/55c66eb5-ce90-4351-8fe4-4bdf843d3556)



# SQL: Performing an SQL query.
In this project, I demonstrated foundational SQL skills by writing and executing queries to retrieve data.

# Environments and Technologies Used.
- Google Cloud Virtual Machines.
- SQL database

# Actions and observations.

In this lab activity, we’ll use the SELECT and FROM clauses in SQL to retrieve the necessary information from a database. We’ll also use the ORDER BY keyword to sequence the information returned by a query based on a specified column.

In this scenario, we have to determine which employee devices must be updated. We also need to investigate user login activity to explore if any unusual activity has occurred. The information we need is located in the machines and login_attempts tables in the organization database.

![image](https://github.com/user-attachments/assets/f750ede9-e0d8-48a3-a905-ab7389c24e31)

- Using SELECT * to retrieve data from the machine's table.
FROM machines;

![image](https://github.com/user-attachments/assets/d6dfc857-70a1-4177-9181-ba98c97b6a34)

- Analyzing data retrieved, we need to see what email client was returned in the third row, which is Email Client 2.

![image](https://github.com/user-attachments/assets/f74e2be3-cf76-49ff-8874-ca54634eca01)

- Using SELECT device_id, operating_systems, OS_patch_date to find the patch date of the first entry.
   -> FROM machines;
