# Database

## What and Why
For my IP I created a Hearthstone Deck Maker. In this application users will be able to view the available cards, create decks and view decks created by other users. Therefor we need a database to store all available cards and created decks. These days a lot of databases are available with different methods of storing the data. So my main question for my research to make a good choice is What database will be best to use for my project?

## How
To execute this research I will make use of the DOT Framework. The DOT Framework consists of 5 research strategies.

![Library](https://ictresearchmethods.nl/images/thumb/8/87/Logo-library.png/50px-Logo-library.png)

Library research is done to explore what is already done and what guidelines and theories exist that could help you further your design. Since the advent of the internet library research is also called desk research.

![Field](https://ictresearchmethods.nl/images/thumb/d/d4/Logo-field.png/50px-Logo-field.png)

Field research is done to explore the application context. You apply a field strategy to get to know your end users, their needs, desires and limitations as organizational and physical contexts in which they will use your product.

![Lab](https://ictresearchmethods.nl/images/thumb/a/ac/Logo-lab.png/50px-Logo-lab.png)

Lab research is done to test parts or concepts of your product, of the final product. You use lab research to learn if things work out the way you intended them, or to test different scenarios.

![Showroom](https://ictresearchmethods.nl/images/thumb/2/22/Logo-showroom.png/50px-Logo-showroom.png)

Showroom research is done to test your ideas in relation to existing work. Showing your prototype to experts can be a form of showroom research or spelling out how your product is different from the competition. Also testing your product to general guidelines is a form of showroom research.

![Workshop](https://ictresearchmethods.nl/images/thumb/e/ea/Logo-workshop.png/50px-Logo-workshop.png)

Workshop research is done to explore opportunities. Prototyping, designing and co-creation activities are all ways to gain insights in what is possible and how things could work.

For my research I will be using the strategy Library research.

## Research Questions

### Which types of database are available?
Designing different types of databases lie at the core of the functionality that they provide to the users. Since data is a dynamic entity, the way it is stored varies a lot. It is also the reason behind companies designing their own types of databases that comply with their needs. For this reason a lot of different type of databases are available and it's hard to keep track of all databases, so I have highlighted 5 of the most common databases, which are:
- Hierarchical databases
- Network databases
- Object-oriented databases
- Relational databases
- NoSQL databases

#### Hierarchical Databases
Just as in any hierarchy, this database follows the progression of data being categorized in ranks or levels, wherein data is categorized based on a common point of linkage. As a result, two entities of data will be lower in rank and the commonality would assume a higher rank. Refer to the diagram below: 
![Hierarchical Database](https://github.com/S3-HSDM/Portfolio/blob/main/images/HierarchicalDB.png)
Do note how Departments and Administration are entirely unlike each other and yet fall under the domain of a University. They are elements that form this hierarchy. Another perspective advises visualizing the data being organized in a parent-child relationship, which upon addition of multiple data elements would resemble a tree. The child records are linked to the parent record using a field, and so the parent record is allowed multiple child records. However, vice versa is not possible. Examples of a Hierarcical database are IBM Information Management System (IMS) and RDM Mobile.

##### Advantages
- Traversing through a tree structure is very simple and fast due to its one-to-many relationships format.
- Easy to understand due to its one-to-many relationships. 

##### Disadvatages
- It’s rigid format of one-to-many relationships. That means, it doesn’t allow more than one parent of a child.
- Multiple nodes with same parent will add redundant data.
- Moving one record from one level to other level could be challenging.

#### Network Databases
In Layman’s terms, a network database is a hierarchical database, but with a major tweak. The child records are given the freedom to associate with multiple parent records. As a result, a network or net of database files linked with multiple threads is observed. Notice how the Student, Faculty, and Resources elements each have two-parent records, which are Departments and Clubs. 
![Network Database](https://github.com/S3-HSDM/Portfolio/blob/main/images/NetworkDB.png)
Certainly, a complex framework, network databases are more capable of representing two-directional relationships. The disadvantage lies in the inability to alter the structure due to its complexity and also in it being highly structurally dependent. Examples of Network databases are Integrated Data Store (IDS) and IDMS (Integrated Database Management System).

##### Advantages
- Conceptual simplicity: Just like the hierarchical model,the network model is also conceptually simple and easy to design.
- Capability to handle more relationship types: The network model can handle the one to many and many to many relationships which is real help in modeling the real life situations.
- Ease of data access: The data access is easier and flexible than the hierarchical model.
- Data integrity: The network model does not allow a member to exist without an owner.
- Data independence: The network model is better than the hierarchical model in isolating the programs from the complex physical storage details.

##### Disadvantages
- System complexity: All the records are maintained using pointers and hence the whole database structure becomes very complex.
- Operational Anomalies: The insertion, deletion and updating operations of any record require large number of pointers adjustments.
- Absence of structural independence: Structural changes to the database is very difficult.

#### Object-oriented Databases
Those familiar with the Object-Oriented Programming Paradigm would be able to relate to this model of databases easily. Information stored in a database is capable of being represented as an object which response as an instance of the database model. Therefore, the object can be referenced and called without any difficulty. As a result, the workload on the database is substantially reduced. 
![Object-oriented Database](https://github.com/S3-HSDM/Portfolio/blob/main/images/ObjectOrientedDB.png)
In the chart above, we have different objects linked to one another using methods; one can get the address of the Person using the livesAt() method. Furthermore, these objects have attributes which are in fact the data elements that need to be defined in the database. An example of this database is Berkeley DB.

##### Advantages
- Complex data sets can be saved and retrieved quickly and easily.
- Object IDs are assigned automatically.
- Works well with object-oriented programming languages.

##### Disadvantages
- Object databases are not widely adopted.
- The high complexity can cause performance problems.

#### Relational Databases
There are dozens of types of databases and one of the most popular database types is relational. A relational database is a DBMS (Database Management Systen) that represents the data in a tabular form of rows and columns. A table is a representation of an entity. Each column in a table represents an attribute of the entity, also known as fields or properties. Each row in a table represents a record, the data associated with an entity. SQL is used to access and manipulate Relational Databases. Each column of a table has a data type that represents the kind of data a column can store. For example, the company name or customer name is a varchar type that can store characters, but a zip code is a numeric field and can store numbers only. Examples of Relational databases are Oracle, MySQL, PostgreSQL and MicrosoftSQL.

A table in RDBMS typically has a unique private key (PK) that uniquely identifies each row in a table. The private key can be a single column or a combination of multiple columns. A primary key ensures that each row in a table is unique. PK is also used as a constraint to force data integrity. A table can contain only one primary key. A foreign key (FK) is a column or combination of columns, that is used to create a relationship between two tables. When a PK is referenced in another table, it is called a foreign key on the referenced table.
![Relational Database](https://github.com/S3-HSDM/Portfolio/blob/main/images/RelationalDB.png)

##### Advantages
- Simplicity of Model: In contrast to other types of database models, the relational database model is much simpler. It does not require any complex queries because it has no query processing or structuring so simple SQL queries are enough to handle the data.
- Ease of Use: Users can easily access/retrieve their required information within seconds without indulging in the complexity of the database. Structured Query Language (SQL) is used to execute complex queries.
- Accuracy: A key feature of relational databases is that they’re strictly defined and well-organized, so data doesn’t get duplicated. Relational databases have accuracy because of their structure with no data duplication.
- Data Integrity: RDBMS databases are also widely used for data integrity as they provide consistency across all tables. The data integrity ensures the features like accuracy and ease of use.
- Normalization: Database normalization also ensures that a relational database has no variety or variance in its structure and can be manipulated accurately. This ensures that integrity is maintained when using data from this database for your business decisions.
- Collaboration: Multiple users can access the database to retrieve information at the same time and even if data is being updated.
- Security: Data is secure as Relational Database Management System allows only authorized users to directly access the data. No unauthorized user can access the information.

##### Disadvatages
- Maintenance Problem: The maintenance of the relational database becomes difficult over time due to the increase in the data. Developers and programmers have to spend a lot of time maintaining the database.
- Cost: The relational database system is costly to set up and maintain.
- Physical Storage: A relational database is comprised of rows and columns, which requires a lot of physical memory because each operation performed depends on separate storage. The requirements of physical memory may increase along with the increase of data.
- Lack of Scalability: While using the relational database over multiple servers, its structure changes and becomes difficult to handle, especially when the quantity of the data is large. Due to this, the data is not scalable on different physical storage servers. Ultimately, its performance is affected i.e. lack of availability of data and load time etc. As the database becomes larger or more distributed with a greater number of servers, this will have negative effects like latency and availability issues affecting overall performance.
- Complexity in Structure: Relational databases can only store data in tabular form which makes it difficult to represent complex relationships between objects. This is an issue because many applications require more than one table to store all the necessary data required by their application logic.
- Decrease in performance over time: The relational database can become slower, not just because of its reliance on multiple tables. When there is a large number of tables and data in the system, it causes an increase in complexity. It can lead to slow response times over queries or even complete failure for them depending on how many people are logged into the server at a given time.

#### NoSQL Databases
A NoSQL originally referring to non SQL or non-relational is a database that provides a mechanism for storage and retrieval of data. This data is modeled in means other than the tabular relations used in relational databases. A NoSQL database includes simplicity of design, simpler horizontal scaling to clusters of machines, and finer control over availability. The data structures used by NoSQL databases are different from those used by default in relational databases which makes some operations faster in NoSQL. The suitability of a given NoSQL database depends on the problem it should solve. Data structures used by NoSQL databases are sometimes also viewed as more flexible than relational database tables. NoSQL databases can be categorized in the following five major categories; Column, Document, GraphKey-value, Object & databases. Examples of NoSQL databases are MongoDB, ArangoDB and CosmosDB.

##### Advantages
- Flexible scalability: They can be scaled horizontally as opposed to vertically, which provides a clear advantage over SQL databases.
- Flexible data types: NoSQL databases allow you to store and retrieve data with only limited or no requirements for the predefined schema. 
- Large amounts of data storage: Many NoSQL databases can handle extensive datasets, making them ideal for big data applications, IoT (Internet of Things), and other real-time analytics.
- Simplicity and less code: Many NoSQL database management systems require only a few lines of code, which is ideal for developers who want to get started quickly.
- Less ongoing database maintenance: NoSQL databases don't require the same level of ongoing database administration as traditional relational databases because they can automatically partition and replicate information across nodes.

##### Disadvantages
- Queries are less flexible: NoSQL databases are more flexible when storing a wide variety of data structures, but they lack the complex query functionality found in SQL.
- Less mature: Since SQL has been around a lot longer, it is generally universal and more mature.
- NoSQL isn't designed to scale by itself: While there are ways to scale out your application using some NoSQL database management systems like BigTable or MongoDB replica sets, their design limits the amount of traffic they can accommodate by themselves.

#### Conclusion
Since I need a database which can handle relationships between entities the NoSQL databases won't satisfy the requirements for my database. The network database also drops out since my database should be able to easily perform the CRUD functions, which need a lot of pointer adjustment in Network databases. The Hierarchical database also drops out because of the lack of multiple types of relationships, it only support one-to-many relations, where I also need many-to-many relations in my project. Then the choice is between Relational and Object-oriented databases. The choice for me goes to a Relational database, since it has moe support in implementing it in my project. The Relational database is more mature and is used way more than the Object-oriented databases.

### Which Relational Databases are available?
The 4 bigger/more popular Relational databases are Oracle, MySQL, MicrosoftSQL Server and PostgreSQL. Of those 4 databases I have used MySQL before and liked MySQL. For me MySQL was easy to setup and use for the projects I have made in the past.

#### Oracle
Oracle has provided high-quality database solutions since the 1970s. The most recent version of Oracle Database was designed to integrate with cloud-based systems, and it allows you to manage massive databases with billions of records. Traditionally, Oracle has offered RDBMS solutions. Today, there are, both, SQL and NoSQL database solutions available.

##### Advantages
- The most advanced technology: Oracle is known for being on the leading edge of database technology. They have a long-standing reputation for bringing quality, along with the latest features and innovations, to their customer base.
- A wide range of solutions: Oracle offers a massive suite of tools and solutions that can address virtually any information challenges you encounter.

##### Disadvantages
- An expensive solution: Oracle tends to be a high-cost solution that smaller, non-enterprise-level organizations might not be able to afford.
- System upgrades might be required: Your current system specifications might not be enough to implement Oracle. Many businesses have to upgrade their hardware before using Oracle solutions.

**Best use case for Oracle:** If you’re a large organization that needs to manage a massive amount of data, Oracle could be the ideal choice.

#### MySQL
MySQL is a free, open-source RDBMS solution that Oracle owns and manages. Even though it’s freeware, MySQL benefits from frequent security and features updates. Large enterprises can upgrade to paid versions of MySQL to benefit from additional features and user support. Although MySQL didn't support NoSQL in the past, since Version 8, it provides NoSQL support to compete with other solutions like PostgreSQL.

##### Advantages
- It’s free: As an open-source RDBMS solution, MySQL is free to use in any way you want.
- Highly compatible with other systems: MySQL has a reputation for being compatible with many other database systems.

##### Disadvantages
- Missing features common to other RDBMSs: Because MySQL prioritizes speed and agility over features, you might find that it’s missing some of the standard features found in other solutions. For example, the ability to create incremental backups.
- Challenges getting quality support: The free version of MySQL does not come with on-demand support. However, MySQL does have an active volunteer community, user forums, and a lot of documentation that you may find useful. 

**Best use case for MySQL:** MySQL is a particularly valuable RDBMS solution for businesses that need a solution with enterprise-level capabilities, but are operating under strict budget constraints. It is an extremely powerful and reliable modern RDBMS with a free tier.

#### MicrosoftSQL Server
MicrosoftSQL Server is a database engine that is compatible with, both, on-site and cloud-based servers. Moreover, there is a Windows and a Linux version of Microsoft SQL. In 2016, Microsoft also added temporal data support. The feature is useful for querying historical data whose state might have changed. Microsoft SQL Server also supports dynamic data masking, which boosts security by masking sensitive information from non-privileged users.

##### Advantages
- It's mobile: This database engine allows you to access dashboard graphics and visuals via mobile devices.
- Integrates with Microsoft products: Companies that rely heavily on Microsoft products will enjoy the way SQL Server integrates easily with these applications.
- It's fast: Microsoft SQL Server has built a reputation around being fast and stable.

##### Disadvantages
- It's expensive: Considering that there are plenty of free database engines available, the cost of Microsoft SQL Server is steep. It's over $14,000 for one enterprise-level license per core. There are scaled-down licensing options for approximately $3,700 and $900, and a free version you can use to test the platform.
- Requires a lot of resources: This resource-heavy RDBMS may require you to purchase better hardware. Here is a review of Microsoft SQL Server that highlights the issue.

**Best use case for Microsoft SQL Server:** If you're an enterprise-level corporation that relies heavily on Microsoft products, the speed, agility, and reliability of Microsoft SQL Server could be an excellent choice.

#### PostgreSQL
PostgreSQL is an open-source, free database engine with unlimited scaling capabilities. PostgreSQL supports both relational and non-relational data formats. As a highly trusted DBMS that has been around since the early 1990s, PostgreSQL has a devoted user base and has won the prestigious Database of the Year Award, twice. An interesting feature of PostgreSQL is its history of working with both structured (SQL) and unstructured (NoSQL) data. PostgreSQL has a catalog-driven approach, which makes it highly extensible. It doesn’t simply store information to identify tables and columns. It allows you to define data types, index types, and functional languages. It's also compatible with most operating systems, including Linux platforms, and it integrates well with data from a wide variety of databases. PostgreSQL also works with, both, on-site servers and cloud-based servers. Even though it's a non-profit, free database system, a large network of devoted followers and volunteers offer free support to users and regularly update the system.

##### Advantages
- More features: PostgreSQL has a lot more features than other DBMSs. These extra features include table inheritance, a rich set of data types (including native support for JSON), ability to define a column as an "array" of column types, among others.
- Highly ACID (Atomicity, Consistency, Isolation, and Durability) Compliant: PostgreSQL consistently ranks as the most ACID-compliant DBMS. If data integrity is your top priority, PostgreSQL could be an ideal choice.
- Massive Scalability: PostgreSQL can work with massive database tables. 

##### Disadvantages
- Lack of documentation: PostgreSQL doesn't have the best documentation compared to other database engines. If you run into an issue, you might need to seek help from a private PostgreSQL support firm, or try your luck with the community support forums.
- Issue of speed with read-only operations: PostgreSQL excels with read-write operations for data that needs validation, but slowdowns could happen when working with read-only operations.

**Best use case for PostgreSQL:** Since PostgreSQL is completely free and scalable, this is an excellent solution for companies of any size. More importantly, if you can benefit from a DBMS with native JSON support, PostgreSQL is for you.

#### Conclusion
Since the Oracle and MicrosoftSQL server aren't for free, those options are ruled out. Therefor two options are left, MySQL and PostgreSQL. For my project I don't need a lot of fancy features, but I need a solution that provides the stored data fast and reliable. Also the lack of documentation for PostgreSQL can be an issue, since I would heavily rely on support of the userbase.

## Conclusion
To answer the main question of my research I would say MySQL is the best fit for my IP. It's free to use, the database has no clunky features, which make it fast and reliable. Also I have used the database myself before and know it's easy and quick to setup. PostgreSQL would be a good alternative, it's also a free to use database, but it focuses more on features. It isn't really clear which of those two databases is faster but PostgreSQL is thought to be faster  for handling massive data sets, complicated queries, and read-write operations. MySQL is thought to be faster with read-only commands, which is the main functionality for my project.

## Sources
[Types of Databases](https://www.geeksforgeeks.org/types-of-databases/) </br>
[What is a Hierarchical Database](https://www.c-sharpcorner.com/article/what-is-a-hierarchical-database/) </br>
[Netwerk model and their Advantages and Disadvantages](http://dbmsenotes.blogspot.com/2014/03/comparison-of-data-models-data-models.html) </br>
[Object-oriented database: Explenation + Advantages & Disadvantages](https://www.ionos.com/digitalguide/hosting/technical-matters/object-oriented-databases/) </br>
[What is a Relational Database (RDBMS)](https://www.c-sharpcorner.com/article/what-is-a-relational-database/) </br>
[Relational Database Benefits and Limitations (Advantages & Disadvantages)](https://databasetown.com/relational-database-benefits-and-limitations/) </br>
[What are the Pros and Cons of NoSQL](https://www.adservio.fr/post/what-are-the-pros-and-cons-of-nosql#:~:text=The%20top%20advantages%20of%20NoSQL,less%20mature%2C%20less%20flexible%20queries.&text=Queries%20are%20less%20flexible.&text=NoSQL%20isn't%20designed%20to%20scale%20by%20itself.) </br>
[Which Database Is Right for Your Use Case?](https://www.integrate.io/blog/which-database/) </br>
[PostgreSQL vs MySQL: The Critical Differences](https://www.integrate.io/blog/postgresql-vs-mysql-which-one-is-better-for-your-use-case/#ismysqlorpostgresqlfaster)
