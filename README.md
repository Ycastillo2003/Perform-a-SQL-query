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

- Using SELECT device_id, -> FROM machines; operating_systems, OS_patch_date to find the patch date of the first entry.
   

![image](https://github.com/user-attachments/assets/405e4000-f8dd-4693-956e-a8e4bdd05dd3)

- Observing the retrieved data, the first patch date entry is 2021-09-01.

![image](https://github.com/user-attachments/assets/7bf52197-19f1-4afe-a785-dd3c9cc0e5bf)

- Using SELECT event_id, country -> FROM log_in_attempts  to investigate login attempts, specifically if any login attempts were made from Australia.

  ![image](https://github.com/user-attachments/assets/496760a2-bc78-4461-968e-f014954c0393) ![image](https://github.com/user-attachments/assets/2325cacd-0151-4b85-9cb5-c66891b2b7ab)![image](https://github.com/user-attachments/assets/fcda6543-df68-4427-bce2-14401593d344)![image](https://github.com/user-attachments/assets/cf1e5d88-a43a-4baf-9b00-cc7c49c7ace2)

- Analyzing all 200 rows and verifying that no login attempts were made from Australia.

![image](https://github.com/user-attachments/assets/4c70c868-5210-4113-a7d3-e6d600ecb357)

- Using SELECT username, login_date, Login_time FROM log_in_attempts to check if any login attempts were made after work hours.

![image](https://github.com/user-attachments/assets/ab11220e-84fa-4e80-a576-83b3ff3c388a)![image](https://github.com/user-attachments/assets/b3b98333-8674-4d24-b542-19b17cd97ce4)![image](https://github.com/user-attachments/assets/02b0d40e-92a9-482f-ad9e-993e6051bb96)

- Observing data and noticing that there were several login attempts made after work hours.

![image](https://github.com/user-attachments/assets/81228c67-b4ae-4540-a592-4ba3c9a33813)

- Now we are going to use an ORDER BY clause to organize our log_in_attempts by date.

![image](https://github.com/user-attachments/assets/edd9f295-2279-400e-9b81-57f73bc74bf7)

- Now our data is more organized however, we are going further to organize the previous results by ordering them by login_time. We will do that by modifying  the query from the previous step by adding the login time to the ORDER BY clause.


