<h1><center>Introduction to MongoDB</center></h1>

##### Authors: 
Fnu Shikha <br>
Monika Krishnamurthy

### Intro: 
MongoDB is a tool that explore data without knowing structure. It is a source available cross platform document-oriented database program. It comes under NoSQL database. <br>
MongoDB works on concept of collection and document. <br>
•	Database: Database is a physical container for collections. Each MongoDB server has multiple databases.<br>
•	Collection: MongoDB collection is a group of documents. It is like tables in RDBMS/SQL databases. A collection exists within single database. MongoDB is different from SQL by stating that collections do not enforce a schema.<br>
•	Document: A document is a set of key-value pairs. Documents have dynamic schema which means that documents in the same collection do not need to have the same set of fields or structure. <br>

![Picture1.png](attachment:Picture1.png)



### Data Format in MongoDB: 
•	JSON(JavaScript Object Notation) is the basis of the data format in MongoDB. <br>
•	JSON has two collection centers: <br>
1. Objects {}: Object map string keys to values. <br>
i.	String keys and values {‘key1’:value1, ‘key2’:’value2’,….}<br>
ii.	 Order of values is not important<br>
{ 
                       ‘id’ : 12345,
                       ‘name’:’abc’,
                       ‘instructor’:true
                        },
2. Arrays []: Arrays order values. <br>
i.	Series of values[value1,value2,….]<br>
ii.	Order of values is important<br>
[
                     “instructor_1”,
                     “instructor_2”,
                       …
                      ]


### MongoDB supports many datatypes. Some of them are –
-	String − This is the most used datatype to store the data. String in MongoDB must be UTF-8 valid.
-	Integer − This type is used to store a numerical value. Integer can be 32 bit or 64 bit depending upon your server.
-	Boolean − This type is used to store a Boolean (true/ false) value.
-	Double − This type is used to store floating point values.
-	Min/ Max keys − This type is used to compare a value against the lowest and highest BSON elements.
-	Arrays − This type is used to store arrays or list or multiple values into one key.
-	Timestamp − This can be handy for recording when a document has been modified or added.
-	Object − This datatype is used for embedded documents.
-	Null − This type is used to store a Null value.
-	Symbol − This datatype is used identically to a string; however, it's generally reserved for languages that use a specific symbol type.
-	Date − This datatype is used to store the current date or time in UNIX time format. You can specify your own date time by creating object of Date and passing day, month, year into it.
-	Object ID − This datatype is used to store the document’s ID.
-	Binary data − This datatype is used to store binary data.
-	Code − This datatype is used to store JavaScript code into the document.
-	Regular expression − This datatype is used to store regular expression.


### Unstructured data: 
Unstructured data doesn’t have a pre-defined model or its not organized as pre-defined manner.

#### Characteristics of unstructured data:
•	Data doesn’t follow any rules or semantics.
•	No Format or structure.
•	No easily identifiable structure and because of that its little tough to use by computer programs easily.
•	Cannot be stored as rows or columns as in Databases.

#### Sources of unstructured data:
•	Web Pages
•	Images (JPEG, PNG, GIF, etc)
•	Videos
•	Memos
•	Reports
•	Word documents

#### Advantages of Unstructured data:
•	It supports the data which lacks proper format or sequence.
•	There is no constraint of schema
•	Data is portable and scalable.
•	Data is very flexible as there is no schema.

#### Disadvantages of Unstructured data:
•	It is difficult to store and manage unstructured dataset as there is no schema and structure.
•	Indexing the data is difficult because of unclear structure and not having pre-defined structures.
•	Due to unclear structure, it is difficult to optimize functions like update, delete etc. in unstructured dataset.

•	Any relational database has a typical schema that shows relationship between tables. While MongoDB doesn’t have the concept of relationship.

#### Advantages of MongoDB over RDBMS:
•	It is scalable.
•	MongoDB uses internal memory for storing the data, hence it enables faster access of data.
•	No complex joins like RDBMS.
•	The most important advantage of MongoDB over RDBMS is, MongoDB is schema less. It means number of fields, content and size of the document can differ from one document to another.


•	Any relational database has a typical schema that shows relationship between tables. While MongoDB doesn’t have the concept of relationship.

#### Advantages of MongoDB over RDBMS:
•	It is scalable.
•	MongoDB uses internal memory for storing the data, hence it enables faster access of data.
•	No complex joins like RDBMS.
•	The most important advantage of MongoDB over RDBMS is, MongoDB is schema less. It means number of fields, content and size of the document can differ from one document to another.



### Example: 
Suppose a client needs a database design for his blog/website and see the differences between RDBMS and MongoDB schema design. Website has the following requirements.<br>
•	Every post has the unique title, description and url.<br>
•	Every post can have one or more tags.<br>
•	Every post has the name of its publisher and total number of likes.<br>
•	Every post has comments given by users along with their name, message, data-time and likes.<br>
•	On each post, there can be zero or more comments.<br>
<br>
In RDBMS schema, design for above requirements will have minimum three tables.<br>
![Picture1.png](attachment:Picture1.png)


While in MongoDB schema, design will have one collection post and the following structure –
![Picture1.png](attachment:Picture1.png)

In RDBMS, we need to join three tables while in MongoDB, data will be shown from one collection only.<br>
•	Where to use MongoDB?<br>
•	Big data<br>
•	Content Management<br>
•	Data Hub<br>

•	Install MongoDB on windows:<br>
##### I.	Go to the below link and click on the Download button.<br>
https://www.mongodb.com/try/download/community
![Picture1.png](attachment:Picture1.png)

##### II.	Follow steps accordingly for download.
![Picture1.png](attachment:Picture1.png)

##### III.	Continue once we see the below pop-up.
![Picture1.png](attachment:Picture1.png)

##### IV.	Once it is downloaded, navigate to the C drive on computer and create a new folder called data here. 
![Picture1.png](attachment:Picture1.png)

##### V.	Create a folder in data as db.
![Picture1.png](attachment:Picture1.png)

##### VI.	Once installation is complete, we need to set up MongoDB on the local system.<br>
•	Open Hyper terminal running Git Bash.<br>
•	Change directory to home directory using <br>
![Picture1.png](attachment:Picture1.png)


•	Create a file called .bash_profile using the following command<br>
![Picture1.png](attachment:Picture1.png)

•	Open the newly created .bash_profile with vim using the following command:
![Picture1.png](attachment:Picture1.png)

•	In vim, hit the I key on the keyboard to enter insert mode.
![Picture1.png](attachment:Picture1.png)

•	In Drive C navigate: C < Program Files < MongoDB < Server<br>
We can see the version of MongoDB. Here, I can see its 5.0
![Picture1.png](attachment:Picture1.png)


•	Paste in the following code into vim, make sure you replace the 5.0 with your version that you see in explorer as in above screenshot.<br>
![Picture1.png](attachment:Picture1.png)

•	Hit the Escape key on your keyboard to exit the insert mode. Then type to save and exit vim.
![Picture1.png](attachment:Picture1.png)

##### VII.	Verify the setup is successful:<br>
•	Close down the current Hyper terminal and quit the application.<br>
•	Re-launch Terminal.<br>
•	Type the following commands into the Hyper terminal and hit enter.<br>
![Picture1.png](attachment:Picture1.png)
•	If terminal shows below details like version details, it shows setup is successful.<br>
![Picture1.png](attachment:Picture1.png)

#### Create Database:
•	In MongoDB, use DATABASE_NAME is used to create database.<br>
![Picture1.png](attachment:Picture1.png)


•	To check current selected database check db and it will give the current database.<br>
•	To check database list, use command ‘show dbs’.<br>
•	In the list mydb is not present because there is no data. First insert data and then again check the database list using above command.<br>
![Picture1.png](attachment:Picture1.png)


#### Drop Database:
-	db.dropDatabase() command is used to drop an existing database. 
![image.png](attachment:image.png)


#### Create collection:
-	db.createCollection(name, options) is used to create collection.
Name is name of collection to be created, options is a document and is used to specify configuration of collection.


#### Drop collection:
-	db.collection.drop() is used to drop a collection from the database.
![image.png](attachment:image.png)

#### Insert data into MongoDB:
-	Insert a new document into collection DSKB. As DSKB is not having id earlier, it will add new field as _id field for the new document. “MongoDB adds the _id field with an ObjectId value to the new document.” 
![image.png](attachment:image.png)

-	Unlike SQL tables, MongoDB collections have dynamic schemas. That is, a single collection can store documents that differ in shapes (i.e. contain different fields and value types). And unlike SQL, no DDL operation is required to add or remove fields or modify field types. You just update the documents directly.


#### Read data from MongoDB using queries:
-	Check data into collection DSKB.
![image.png](attachment:image.png)
-	Using InsertMany:
![image.png](attachment:image.png)
-	Find data for only status = D
![image.png](attachment:image.png)

# References:
https://docs.mongodb.com/guides <br>
https://www.tutorialspoint.com/mongodb/index.htm <br>
https://campus.datacamp.com/courses/introduction-to-using-mongodb-for-data-science-with-python

