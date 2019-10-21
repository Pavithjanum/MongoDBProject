# MongoDBProject
MongoDB Project

MongoDB is a high-performance, scalable, distributed database designed for a wide variety of modern applications. It is used by organizations of all sizes to power mission-critical, operational applications where low latency, high throughput, and continuous availability are critical requirements of the system.
As with any database, applications deployed on MongoDB require careful planning and the coordination of many roles in an organization's IT team to ensure successful deployment and operation. Developers and data architects should work together to develop the right data model, and should invest time in this exercise early in the project.
The below project would challenge you on end-to-end implementation of MongoDB, considering the best practices and selecting the best approach. You would utilize various skills, options, techniques and features you have learnt throughout this course to solve the problem statements. Each problem statement will challenge you to think and decide a solving approach. You would be provided with some high-level steps to ensure your approach is correct.

Problem Statement 1
In an e-commerce company, customers browse the website to place orders for various brands and items. In the process, they must register themselves, sign in with a username and password, search for specific brands and items, and place an order. While placing the order they can add/remove products from the shopping cart, discard the shopping cart, or proceed with the payment using various payment options.
The data stored from all the transactions and activities happening on the website is complex in nature. It could be in structured or unstructured format. It might be in text, document, or JSON format. Being the Database Administrator of your organization, you are responsible to use a database which has flexible schema, reduces the operational procedure, and is highly scalable and reliable.
Approach
Installation and Configuration of MongoDB:
1. Download the MongoDB setup
2. Install MongoDB
3. Configure the Mongo Shell
4. Scripting through Mongo Shell

Problem Statement 2
Further after the installation and configuration of the database, you must identify the final data schema. To do so:
• Identify the operations that the system need to support, based on the system functionality
• Identify the entities that the operations 'interact' with
• Identify meta-data of the entities
• View how the entities are used in the system in relation to one another
• Bring it all together by using the findings from the above steps and apply some best practice rules to them.
Approach
Observe and analyse the data (provided with this Project Statement) to determine which schema would be appropriate to store it in MongoDB.

Problem Statement 3
After you create a logical schema, next step is to create a database named as “Mongo_DB_Project” which would be handled by a user “Adam”. You must maintain orders, customers and categories of data with brands and items in segregated form. You are also responsible for modifying the documents and removing duplicate or redundant documents.
Approach
1. Create Database “Mongo_DB_Project” using “use DBName”
2. Create User with roles:
db.createUser({
user: "Adam",
pwd: "adam",
roles: ["readWrite","dbAdmin"]
});
3. Create 3 Collections as below:
a. Orders: Order details and item details
b. Categories: Categories with brands and items details
c. Customers: Customer details with Items
4. Insert documents in the collections
5. Query data from MongoDB using find command

6. The price of Dell OptiPlex computer has increased from 32200 to 33000. Update the document in Category collection accordingly.
7. Observe the documents to find a duplicate document with different order_id.
8. Delete the duplicate document(s).
Problem Statement 4
Your organization keeps consolidated data in a single file for all categories with distinct brands and items for each brand with item details. So, you must take a backup of the data.
Approach
1. Backup a database with mongoexport
2. Restore the data using mongoimport
Problem Statement 5
With the increasing data, the query performance of MongoDB has declined. You are responsible for optimizing the query performance of the database. Which steps would you take?
Approach
Perform indexing
Problem Statement 6
Your manager has asked you to provide total price obtained from order placed for various items.
Approach
Perform aggregation functions

Problem Statement 7
With the modernization of technologies, you should also modernize the storage process of the organizational data to increase flexibility and scalability at reduced cost. So, you decide to host your database somewhere and deploy it to make it secure, fast and highly available for any scale. You suggest your managers that you can save your data in MongoDB Atlas. So, you are now responsible to store your data in MongoDB Atlas and provide security to your cluster.
Approach
1. Create a Cluster in MongoDB Atlas
2. Store your data in a Stitch Application

Problem Statement 8
You have a lot of unwanted, empty and invalid collections which are consume the memory space of the server machine. Some users have also complained about some warnings and errors encountered while performing various tasks. What would you do?
Approach:
Run Diagnostic commands
Problem Statement 9
The developer of your organization has created a new application. You are asked to perform a test for the same application, where you will insert few documents in MongoDB database using a Rest Client.
Approach
1. Install the Drivers in your system.
2. Save the .war file in your system and use POSTMAN application to connect your application with MongoDB database.
Problem Statement 10
As a database Administrator, you must be well prepared to face situations like system failure, disaster management recovery. You should have replica sets created of your server database.
Approach
1. Create primary replica and secondary replica
