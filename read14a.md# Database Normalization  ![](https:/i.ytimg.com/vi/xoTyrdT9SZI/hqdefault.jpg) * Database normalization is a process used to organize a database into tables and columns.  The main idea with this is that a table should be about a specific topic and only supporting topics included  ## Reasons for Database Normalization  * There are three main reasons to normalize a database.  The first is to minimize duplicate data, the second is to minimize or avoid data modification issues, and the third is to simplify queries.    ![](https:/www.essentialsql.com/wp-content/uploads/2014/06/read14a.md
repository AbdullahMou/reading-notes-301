# Database Normalization

![](https://i.ytimg.com/vi/xoTyrdT9SZI/hqdefault.jpg)
* Database normalization is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included

## Reasons for Database Normalization

* There are three main reasons to normalize a database.  The first is to minimize duplicate data, the second is to minimize or avoid data modification issues, and the third is to simplify queries. 


![](https://www.essentialsql.com/wp-content/uploads/2014/06/Intro-Table-Not-Normalized.png)

* The first thing to notice is this table serves many purposes including:

  * Identifying the organization’s salespeople
  * Listing the sales offices and phone numbers
  * Associating a salesperson with an sales office
  * Showing each salesperson’s customers

## Data Duplication and Modification Anomalies

* Notice that for each SalesPerson we have listed both the SalesOffice and OfficeNumber. There are duplicate salesperson data. Duplicated information presents two problems:

  * It increases storage and decrease performance.
  * It becomes more difficult to maintain data changes.
* Consider if we move the Chicago office to Evanston, IL. To properly reflect this in our table, we need to update the entries for all the SalesPersons currently in Chicago.  Our table is a small example, but you can see if it were larger, that potentially this could involve hundreds of updates.

* These situations are modification anomalies. Database normalization fixes them. There are three modification anomalies that can occur:

### Insert Anomaly

* There are facts we cannot record until we know information for the entire row.  In our example we cannot record a new sales office until we also know the sales person.  Why?  Because in order to create the record, we need provide a primary key.  In our case this is the EmployeeID.

### Update Anomaly

* In this case we have the same information in several rows. For instance if the office number changes, then there are multiple updates that need to be made.  If we don’t update all rows, then inconsistencies appear.

### Deletion Anomaly

* Deletion of a row causes removal of more than one set of facts.  For instance, if John Hunt retires, then deleting that row cause us to lose information about the New York office.

## Search and Sort Issues

* The last reason we’ll consider is making it easier to search and sort your data.  In the SalesStaff table if you want to search for a specific customer such as Ford, you would have to write a query like

  * `SELECT SalesOffice`</br>
`FROM SalesStaff`</br></br>
`WHERE Customer1 = ‘Ford’ OR`</br>
      `Customer2 = ‘Ford’ OR`</br>
      `Customer3 = ‘Ford’`
* Clearly if the customer were somehow in one column our query would be simpler.  Also, consider if you want to run a query and sort by customer. 

## Definition of Database Normalization

* There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively. 
  
  * First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
  
  * Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
  
  * Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key
