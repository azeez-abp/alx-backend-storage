
# Starting the SQL Mysql analysis
## A database is an organized **collection of structured data**, usually controlled by a database management system (DBMS)
## Operation related
- SQL Has Commands which are
 - - Data Definition Language(define the database schema)
 - - Data Query Language (performing queries on the data within schema objects)
 - - Data Manipulation Language (manipulate data present in the database )
 - - Transaction Control Language (set of tasks into a single execution unit)
 - - Data Control Language. (control access to data stored in a database (Authorization))

- Installation

- User access  use (Data Control Language)
```
CREATE USER 'user_name'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password_of_your_choice';
GRANT PRIVILEGE ON database.table TO 'username'@'host';ALTER USER 'root'@'localhost' IDENTIFIED BY 'root';

Granular access

GRANT  CREATE, ALTER, DROP, INSERT, UPDATE, INDEX, DELETE, SELECT, REFERENCES, RELOAD on *.* TO 'sammy'@'localhost' WITH GRANT OPTION;

WITH GRANT OPTION. This will allow your MySQL user to grant any permissions that  it has to other users on the system.



Column privileges a

GRANT 
   SELECT (employeeNumner,lastName, firstName,email), 
   UPDATE(lastName) 
ON employees 
TO bob@localhost;


SHOW GRANTS FOR 'user_name'@'localhost';
SHOW GRANTS FOR 'user_name'@'localhost';
REVOKE ALL PRIVILEGES ON *.* FROM 'user_name'@'localhost';
REVOKE ALL PRIVILEGES ON *.* FROM 'user_name'@'localhost';

```
- **Database**

```
Type
Hierarchical databases (data categorized in ranks or levels)
Network databases (network database is a hierarchical database, but with a major tweak. The child records are given the freedom to associate with multiple parent records)
Object-oriented databases (Information stored in a database is capable of being represented as an object which response as an instance of the database model.)
Relational databases (every piece of information has a relationship with every other piece of information)
Cloud Database
Centralized Database
Operational Database
NoSQL databases


``` 
- - Enter into db ```mysql -u root -p ``` 
- - show database;
- - use <database_name>; 
- - ALTER DATABASE <current_database_name> MODIFY NAME = <new_database_name>;
- **Table**
- -  show tables;
- -  describe <table_name>;
- -  CREATE, SELECT, UPDATE, DELETE TRUNCATE
- View
- Rows And Column

