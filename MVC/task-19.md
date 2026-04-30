1-MVC pattern:

what is the only part of the
application that should be allowed to talk directly to the
database? 

-Model

Why??
Because it is responsible for
1.Handling data
2.Managing queries of database

-------------------------------------------------------------
2-

Why should sensitive information (like database passwords)
be stored in a separate configuration file instead of being
hardcoded in your main application files??

1.More Secure ==> Configuration files can be protected, encrypted, or excluded from public repositories using files like (.gitignore).
2.Make code clean ==> Keeps the application more organized and easier to read.
3.Environment Flexibility ==> Allow easy switching between environments

---------------------------------------------------------------------------------------
3-
What is PDO in PHP??
- PDO --> PHP Data Objects
- used to connect and interact with databases using a consistent interface.

why is it preferred over older methods like mysqli??

because
1.supports multiple database types 
2.uses an object-oriented ==> easier to maintain and read.
3.helps prevent SQL Injection attacks

------------------------------------------------------------------------------------
4-

How do "Prepared Statements" protect your website from SQL
Injection attacks?

-by separating the SQL query structure from the user’s input data.

----------------------------------------------------------------------------------
5-
When you query a database, you can fetch a single row or
multiple rows. Give a real-world example of a situation where
you need just one row, and a situation where you need an
array of multiple rows.

Single Row ==> In hospital when doctor wants to open patient‘s file Using Id

SELECT * FROM patients WHERE patient_id = 5

Multiple Rows ==> In a Academy when student wants to see all the courses.

SELECT * FROM courses WHERE student_id = 5





















