# Introduction to Database 

## Introduction to Database 

### What is Database ? 
We use database to store data or we say information which we input from users and other type of data like videos, photos, information , comments etc. This all information are stored in a database. 

#### All the type of Application needs good database the points of good database are :- 
 1. Have good Storage to store data.
 2. Have faster computation on our data.
 3. Have queries for our data.

#### Summary :- 
***Database was the solution to store our data it acts as a storage where our data reside and have queries to compute on our data***

## File Base System 

### The Concept of File Based System 
In 1950s we are introduced with file based system which create the hype over the market and it was really very helpful at that time we can store our data very efficiently and easily with that file based system. 

#### Design to store data in file based System :- 
let assume that like our machine storage 
```
            Drive D 
                |____ My-File-one
                            |____ fileOne.txt
                            |____ fileTwo.txt
                            |____ fileThree.txt
```

or 
` Drive D/My-File-One/fileOne.txt,fileTwo.txt,fileThree.txt  `

**When new technology comes people like that technology and not problem with that when times goes the problem comes because technology becomes older** 

### Drawback of File Based System :- 

#### 1. The most important of file based system was Redundancy 
The redundancy was the main concern of file based system let assume that it was file based system so if we saved the information of any person name was Aayush Vyas in fileOne and later if we save the same person Aayush Vyas in fileThree so here we create duplicate of our information and we save the older information in fileOne.txt and new information of same person Aayush Vyas in fileThree.txt.   
**If we do CRUD Operation on this file and READ The Information oF Aayush Vyas and it was Reading information from fileOne so it was reading stale or older information so it create**` Anamoly of Read Operation similarly create Update Anamoly , Create Anamoly, Delete Anamoly also.` 

#### 2. The Security was comparitevly less
The security was less at that time if we compare to this generation Technologies.

#### 3. Scaling File base system was very tough
To Scale our Database we have to use and deal with programming language like c, c++ , java and machine level language like fortrain etc to code and learn this language was difficult because they are machine language so it's tough. 

**We known that the new technologies are pretext challenges of past technologies** 
#### The Challenges are :- 
1. File Base System Created the Redundancy 
2. Complex to Queries over the Database because we have to deal with programming language
3. Less Secure as we compare to new technologies.

### To overcome from this we Drawbacks The New Technologies was created which was Database Management System.

## Database Management System :-
The best Database Management System are MYSQL , ORACLE this both are not Database this are Management System to our Database which has phyiscal layer of database also.

**The Database Management System are the Managemenet system for our database in which our phyiscal layer of databse was wrap which management system or we say layer of code and our database was inside this layer of code.**   

### DBMS was Solve The Drawbacks of File-base-system :- 
**1. It does not occur Redundancy because of management system**  
**2. It was Secure or We Have Security**  
**3. Ease to Use**  
**4.Interact with database become easy because it have it's own query language.** 

### Features Provided by Database Management System 
**1.Scaling and interact with Database become easy because in "DBMS" we don't have to learn complex programming language because it has it's own query language which create queries easy and that language which give by DBMS was "Structured Query language".**  
**2. The Big Problem was Redundancy of file-base-system which solve in Database system Management because here we are don't directly interact with Database because our phyiscal layer of database was covered or wrap with layer of code which decide where this data was stored in our databse.**  
**3. Security concern was also solved here also because it has multiple layer of code so which make our data more secure and security streamlined.**  

## Internet changing the global World 
In 20010 the internet was introduced new world by starting online ecommerce website , online cab system , socail media sites from there the problem of programming also solve for real world 

### Deal with real world problems in program 
To deal with real world problems we think like real world we create **Entities** which are living beings and non-living beings and what was **Relationships** are between them to solve the real problem and we name this solving method paradigam called **Object Oriented Programming** or **OOPS**

### Upgrade in DBMS 
After the Internet revolution we upgrade our Database Management System and and Relationship concept and name that `RDBMS which means Relational Database Management System`.   
**The RDBMS databse are MYSQL , ORACLE etc.** 

#### In RDBMS we stored data in relations here the relations means `Table`.
#### In RDBMS the Data was store in table which was 2D Matrix which has Rows and Columns where `Rows represent Entities` and `Column represent Attributes`

### Assume that you are creating Database of Ecommerce Website :- 
#### We need two things for ecommerce site first was orders and customer 
 **Orders**                         
 - order-id                          
 - client-id                         
 - order-value or order -price
 - order-item  

**Customer**
- customer-id
- customer-name
- customer-address

####  both Information Order and Customer stored in RDBMS Stored in Table :---
_***Order Schema***_  
```
order-id | client-id | order-value or order-price | order-item |  
   1     |  xyz      |   xyz                      |   xyz      | ----> This Row represent Entities  
This Column represent Attributes or Relation  
```
_***Customer Schema***_ 
``` 
customer-id | customer-name | customer-address |  
     1      |    xyz        |   xyz            | ----> This Row represent Entities  
     This Column represent Attributes or Relation
```

## Schema 
The Schema are called to the design and thinking of our Database  
```
In our Application 
----> In our RDBMS 
             ----> We create proper tables rows and columns and types of it 
                                                                        ----> relationships of them 
``` 

### Introduction to Data Model :- 
let understand Data model with example  
Assume that we have to design Data Model of Zoom Car let think what entities we want.... 
```
_Customer________________
| customer :-           |
| customer-id           |
| customer-name         |----------------------
| customer-address      |                     |
|_______________________|                     |
                                              |
_Vechile_________________                     |  
| Vechile :-            |                     |
| vechile-id            |                     |
|  vechile-company      |<---------------------                   
| vechile-model         |
|_______________________|-----------------------
                                               |
_Payments_____________________                 |
| Payments :-                |                 |
| customer-id                |                 |
| customer-card              |                 |
| customer-upi               |                 |
| customer-payment           |<-----------------
|____________________________|------------------
                                               |
___Order_______________________                |
| Order :-                    |                |
| order-id                    |                |
| order-value or order-price  |                |
| order-item                  |<----------------
|_____________________________|

```
`In above we create relationship between our entities so that work our Data Models do it create realtionships between our data model.`

#### So the Data Model will reperesent Entities int the form of Table and Relationship between them. 

### Different type of Relationship 
 1. **One to One Relationship :-**
 In this relationship only one and one entities or only two pair entities are create relationship between them for example  

 ```
 _________________________________________
 | order-id          |     order-name     |
 | #123487           |       XYZ          |
 | #987654           |       ABC          |
 |_#234655___________|_______QWE__________|
 ```
 **Now we have to assign unique order-id to every orders so it was one to one relationship of Relational**

2. **Many to Many Relationship :-** 
A many-to-many relationship occurs when multiple records in one table are associated with multiple records in another table. To establish this relationship, a junction table (or associative table) is used.  
Here's an example using **"Students"** and **"Courses"** tables, where a student can enroll in many courses and a course can have many students.  

```
 Student Table 
 _____________________________________________
 |  RollNumber       |      Student Name     |
 |      1            |     Sam Curran        |                         
 |      2            |      Sam Billings     |
 |      3            |     Tom Moddy         |
 |______4____________|______Joss Butler______|     

 Coures Table 

 ___________________________________________
 |  Subject-code    |       Subject-name   |
 |     m01          |       Mathematics    |
 |     sc02         |       Science        |
 |     en03         |      English         |
 |_____hin04________|______Hindi___________|                        
```

**Now one Students should choose multiple Subjects and one Subjects are choose by multiple Students** 

```
Student-Courses (Table) {Junction of above Two table}

_______________________________________________________
| Student Rollnumber         |    Select Subject       |
|         1                  |      m01                |
|         1                  |      hin04              |
|         1                  |      en03               |
|         2                  |       m01               |
|         2                  |      sc02               |
|         3                  |       sc02              |
|_________4__________________|_______hin04_____________|
```
`In above table we see that one student choose multiple subjects and onse subjects was choose by multiple students this was many to many relationship.`  

3. **One to Many Relationship :-**  
A one-to-many relationship occurs when a single record in one table can be associated with multiple records in another table. A common example is the relationship between "Customers" and "Orders" where each customer can have multiple orders.
```
Customers Table :---
__________________________________________________
|   Customer ID          | Customer Name         |
|      #0001             |     Aayush            |
|      #0002             |     Sumedh            |
|      #0003             |     Rahul             |
|______#0004_____________|_____Chetan____________|
 
 Customer Order Table 
 
 _________________________________________________________________
 | Order-ID   | Customer ID            |     Order-Detail         |
 | #or01      |  #0001                 |   Order detail of #or01  |
 | #or02      |  #0001                 |   Order detail of #or02  |
 | #or03      |  #0002                 |   Order detail of #or03  |
 | #or04      |  #0002                 |   Order detail of #or04  |
 | #or05      |  #0002                 |   Order detail of #or05  |
 | #or06      |  #0003                 |   Order detail of #or06  |
 |_#or07______|__#0004_________________|___Order detail of #or07__|

```

**In Above Example we see that per customer will  order multiple Orders and it was perfect explanation of one to Many Relationship.**


### Key Features of Relational Database Management System "RDBMS"
1. In RDBMS we create Relations by Creating Table 
2. In RDBMS we maintain the Relationship which was maintain by forieng-keys
3. It has feature which was Transcation system which strengthed the RDBMS Today also there was so many competetive DBMS but MYSQL , Oracle now also relaible most of banks are used this technologies.
4. RDBMS was design on the Normalization concept which decrease the chances of redundancy there was some type of normalization which was 1nf , 2nf , 3nf , bcnf.

### Usecase or Scenario of RDBMS 
- **If you need Transcation than the only data we have to use was RDBMS**
-  **If your Data was Structured and we don't have to quickly change our Schema**
- **If we want to make Relationship between Antities than we have to RDBMS**

### Challenges with RDBMS :- 
1. **If our columns are not fixed than RDBMS was not a good choice**  
For example we create Schema of E-commerece and frequently we have to change our Items Entities to add more product than we don't have to use RDBMS here.  
2. **RDBMS are not for huge Dataset**  
If the Data was huge and store in single machine than we can say for example we have huge dataset and we can store in our machine than our queries become slow because we have bigger data or the data which was stored in multiple machine so RDBMS have to use JOIN queries and also use netwrok I/O {Input / Output} which was slowest so here RDBMS are not fit in this case.  

**RDBMS are having this two main challenges which are `Dynamic Schema of DB` and `If the Data was Huge Performance was going down`.**  
### To Overcome this Challenges of RDBMS the new Database was designed which was `NO-SQL database` 

## NO-SQL Database 
The new Database design which was NO-SQL Database which does-not means **Anti-SQL** and **Anti-RDBMS** instead there was other technology with SQL also we conclude that in **no-sql database there was other technology also not only sql.**  

### Types of NO-SQL Database 
1. **Key-pair Value Database**  
In this databse we store our data in key-pair value like Javascript Objects or JSON file example of this database was **Redis**  
2. **Documentation database**  
In this database we store our data in documentation likely in JSON file example of this database was **MongoDB**  
3. **Columnar Database**  
In normal Database the data was stored in rows but in Columnar Database the data was stored in Column the example of database was **Cassandara**  
4. **Graph Database**  
In graph base database we save our data in the form of graphs vertices and edges and the example of graph database was **Neo4J**  
The Graph Database was used in Linkedin application where we saved the complex data in the form of vertices and edges.  



