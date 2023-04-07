# DareIT - cloud_challenge
# 5. Create Cloud SQL

Task 5 point 3 - what is average age of the students in the class?
My answer: 29.5

Knowledge Base: database, database management system (or DBMS), types of Databases, SQL - Structured Query Language, Domain Name System (DNS), Encryption.

TOOLS: 
- Google Cloud Platform
- DBeaver (to be able to connect to the Database)

TASK 5
You will now learn how to create Cloud SQL instance.

Step 1
Go go GCP Console and find Cloud SQL.

Step 2
We will now customise the instance. Choose Connections

Step 3️
Click on your instance, under the General you will be presented with information about how to connect to the instance. You will need the Public IP Address . So copy that address.

Step 4 
Let’s now use Dbeaver to connect to the database and play with data a little bit.
Open Dbeaver, on the left hand side in the white space use right click to and then choose Create New Folder

Step 5
Click Advanced options. And then Networking. Add a network tag dareit-public . This tag will be used to match firewall rules to the instances to which the rules should apply.

Step 6
So what now?
1. Add one more column to the students table called age with type int
2. Add 5 more rows to the table with some proper data. So information about 5 more students.
3. Prepare a query that will answer the question what is average age of the students in the class?
My answer: 29.5
4. Extract to txt data from the students table.
5. Create a new folder in your cloud_challenge repo with name task_5 , commit the txt file there. Add a readme.md with the answer to question from point 3.
6. And remember, Google is your friend! 🎉