Implementation of Evans cycle Logical database

After completing our logical data modelling, I began with our physical design. Here I first made the decision on how to translate entities into tables, the instances into rows and the attributes into columns.  Secondly, i decideded what indexes to define on the tables, which columns of the tables to define as keys, what views to define on the tables, how to de-normalize the tables and how to resolve the different types of relationships. I used a specific database management system MYSQL (Structured query language) to implement my Evans cycle logical database. MYSQL is a standard language for accessing (storing and retrieving) and manipulating databases. It turns raw data stored in a database into actionable insights. 

I started first by setting up the MYSQL community server in my system to create the database schema. A database schema are the blue prints of databases. It shows a database design such as what tables are included in the database and any relationship btw its tables. It lets one know what data type each field can hold. A database schema is first created before the table is created.


To create the database schema, I right clicked on "database" on the left hand of MYSQL work bench and click on create schema. This created a new_schema tab, I named the schema "Evans cycle" then I clicked on apply and finish. After which I clicked on the schema, clicked on tables, right clicked on tables and clicked on create table. A new table tab poped up which I named as customer, then I filled the attributes and the datatypes. I also selected the "customer_id" to be the PRIMARY KEY to uniquely identify each row in the table.

Next, I added constraints to some of the attributes. These constraints specify rules for the data in the tables and controls what can be inputted into the DBMS. I added a NOT NULL constraint to the attributes first_name, last _name and phone number in my "customers"  table so that the table will not accept a record where those attributes are set to "NULL". This is because the "customers" table would require a first name, last name and phone number. I also set email to be "UNQUE" to ensure every record must have a different value for this attribute. 
After adding constraints, I established relationships between the tables by setting up foreign keys. I used the ALTER Table followed by the name of the participant table to update the table. Next, I used the ADD foreign key followed by the attribute to reference the Primary key. 
I created tables for the other entities (orders, staff, stores and order_items) in my Evans cycle logical database. Now that I have all of my tables created in a fully functioning relational database, I populated the tables with data by using the INSERT INTO statement with the table name followed by the data I want in parentheses. The syntax is "INSERT INTO table VALUES (data I want to insert, separated by commas)". I retrieved the data from the database using the SELECT statement. To retrieve all the columns from the database, I used SELECT with an asterisk while to select only some columns, I used SELECT statement followed by the names of the columns I want separated by a comma. 

Below is my “customers table” syntax:

CREATE TABLE `customers` (

  `id` int NOT NULL,
  
  `first_name` varchar(45) NOT NULL,
  
  `last_name` varchar(45) NOT NULL,
  
  `phone_number` varchar(45) NOT NULL,
  
  `email` varchar(45) NOT NULL,
  
  `city` varchar(45) DEFAULT NULL,
  
  `street` varchar(45) DEFAULT NULL,
  
  PRIMARY KEY (`id`),
  
  UNIQUE KEY `email_UNIQUE` (`email`)
  
);

DESC customers;

INSERT INTO  customers VALUES(1,'PRINCE','OKOLIE','07036126160','PINO@YAHOO.CA','JOS','KASHIM IBRAHIM');

SELECT * FROM  customers;


In summary, the primary purpose of data modeling is not to design a database; rather, it is to describe a business. It provides the conceptual understanding and clarity needed to describe a business, while database design translates that understanding into a concrete database structure. Data models serve as a bridge between business requirements and technical implementation. The primary purpose of designing a database is to produce physical and logical models of designs for the proposed database system. Database design focuses on creating the actual structure of a database system. It involves defining tables, relationships, constraints, and indexes. Database design is dependent on the specific DBMS (Database Management System) and the hardware it runs on. Both are essential for effective data management and successful business operations. 
