# Data management and database strategy 

# 1.- We need to design a solution that allows us to receive information from Internet of Things (IoT) sensors at a frequency of millions of requests per second. Which kind of database would you use to be able to support this frequency? 

- a) BigQuery 
- b) **Bigtable** 
- c) Firestore 
- d) Cloud Spanner 

## 2.- You need to implement a solution that can support the consumption of data from the US, Europe, and Asia, maintaining the same experience for different users and allowing transactional operations. Which type of database would you use to accomplish this task?

- a) Cloud SQL 
- b) BigQuery 
- c) Cloud Spanner 
- d) Bigtable 

## 3.- You are asked to implement a database that allows you to scale to zero if no one is using the application, to reduce costs. Which type of database would you use to fulfill this request? 

- a) BigQuery 
- b) Bigtable 
- c) Firestore 
- d) **Cloud Spanner** 

## 4.- You have been commissioned to design the keys of a solution that will be implemented in Bigtable. What should you do to avoid hotspotting on your database? 

- a) Create partitions for each key. 
- b) **Create indexes for each key.** 
- c) Avoid using braces with a sequential increment. 
- d) Do not use compound keys. 

## 5.- You have been asked to create a counter in your application that can receive write operations with a frequency greater than 1 second using Firestore. Which strategy would you use to avoid having contention problems within Firestore? 

- a) Composite index 
- b) Distributed counters 
- c) Document partition 
- d) Split collections