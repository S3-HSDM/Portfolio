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

For my research I will be using 2 of the strategies, Library and Workshop research.

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
- Operational Anomalies: The insertion,deletion and updating operations of any record require large number of pointers adjustments.
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
There are dozens of types of databases and one of the most popular database types is relational. A relational database is a DBMS (Database Management Systen) that represents the data in a tabular form of rows and columns. A table is a representation of an entity. Each column in a table represents an attribute of the entity, also known as fields or properties. Each row in a table represents a record, the data associated with an entity. SQL is used to access and manipulate Relational Databases. Each column of a table has a data type that represents the kind of data a column can store. For example, the company name or customer name is a varchar type that can store characters, but a zip code is a numeric field and can store numbers only. Examples of Relational databases are Oracle, MySQL, PostgreSQL and MariaDB.

A table in RDBMS typically has a unique private key (PK) that uniquely identifies each row in a table. The private key can be a single column or a combination of multiple columns. A primary key ensures that each row in a table is unique. PK is also used as a constraint to force data integrity. A table can contain only one primary key. A foreign key (FK) is a column or combination of columns, that is used to create a relationship between two tables. When a PK is referenced in another table, it is called a foreign key on the referenced table.
![Relational Database](https://github.com/S3-HSDM/Portfolio/blob/main/images/RelationalDB.png)

##### Advantages

##### Disadvatages








#### Conclusion


## Conclusion


## Sources
[Types of Databases](https://www.geeksforgeeks.org/types-of-databases/) </br>
[What is a Hierarchical Database](https://www.c-sharpcorner.com/article/what-is-a-hierarchical-database/) </br>
[Netwerk model and their Advantages and Disadvantages](http://dbmsenotes.blogspot.com/2014/03/comparison-of-data-models-data-models.html) </br>
[Object-oriented database: Explenation + Advantages & Disadvantages](https://www.ionos.com/digitalguide/hosting/technical-matters/object-oriented-databases/) </br>
[What is a Relational Database (RDBMS)](https://www.c-sharpcorner.com/article/what-is-a-relational-database/) </br>


