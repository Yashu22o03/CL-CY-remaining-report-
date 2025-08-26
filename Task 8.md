## Task 8: Database task - DynamoDB

DynamoDB is a fully managed NoSQL database service provided by AWS. It's designed for applications that need single-digit millisecond latency at any scale, making it ideal for high-performance applications where response time is critical.

### Key Concepts:
1. **NoSQL Database :** DynamoDB is a NoSQL database, which means it doesn't use the traditional rows and columns structure like SQL databases. Instead, it stores data in a flexible format.
2. **Managed Service :** AWS manages DynamoDB for you, handling tasks like hardware provisioning, setup, configuration, replication, backup, and scaling. This allows the developer to focus more on application logic rather than database management. 
3. **Data Model :** Data is DynamoDB is stored in tables, which are collections of items. Each item is a collection of attributes, similar to rows and columns in a relational database, but with more flexibility.
4. **Primary Key :** Each table in DynamoDB must have a primary key, which uniquely identifies each item in the table.
5. **Attributes :** Items in DynamoDB can have different attributes, which are similar to fields or columns in a traditional database. Each attribute can be a scalar (like a number, string, or binary) or a complex data type (like lists or maps).


### Usage :
- *Scalability :* DynamoDB automatically scales throughput capacity to handle any amount of traffic, from a few requests per second to millions of requests per second, without requiring manual intervention. 
- *Performance :* It offers consistently low -latency performance, making it suitable for real-time applications like gaming, IoT, mobile apps, and more.
- *Integration :* DynamoDB integrates seamlessly with other AWS services enabling developers to build scalable and resilient applications.


**MySQL :** It is a relational database that stores data in tables with rows and columns, uses SQL for queries, and requires a fixed schema


**NoSQL :** It is a non-relational database that stores data in flexible formats like key-value pairs or documents. It is designed for scalability and handling large, unstructured data. 


### Difference between NoSQL and MySQL 

| Feature        | NoSQL                     | MySQL      |
| -------------- | ------------------------- | ---------- |
| Data Structure | Tables (rows and columns) | Key-value  |
| Schema         | Fixed                     | Flexible   |
| Query Language | SQL                       | Varies     |
| Scalability    | Vertical                  | Horizontal |

I developed a simple user login system that uses AWS DynamoDB to securely store and validate user credentials. The login system includes a web-based user interface built with Flask, allowing users to register with multiple fields and log in using their credentials. 

I learnt how to set up and configure AWS CLI (Command Line Interface), work with Boto3 (AWS SDK for Python) and perform basic operations in DynamoDB.

Below is the VS-Code terminal output :
[![Screenshot-2025-05-29-204208.png](https://i.postimg.cc/595ZPxYG/Screenshot-2025-05-29-204208.png)](https://postimg.cc/w3vfMYkc)
Below are the images of my web-based user interface login system : 
[![Screenshot-2025-05-29-214125.png](https://i.postimg.cc/nrxNHW50/Screenshot-2025-05-29-214125.png)](https://postimg.cc/HcS6z6Ty)

 [![Screenshot-2025-05-29-214153.png](https://i.postimg.cc/T1cFh9vG/Screenshot-2025-05-29-214153.png)](https://postimg.cc/H8VBhbLP)



