# Databases and event messages in Google Cloud

## 1.- You are developing an e-commerce platform where each of the products has different information, based on a semi-structured scheme. Which type of database would you use to store the information? 

- a) BigQuery 
- b) Bigtable 
- c) **Firestore**
- d) Cloud Storage 

    Explanation: Firestore, due to its NoSQL nature and flexible schema, allows us to store different data in our documents in order to fulfill this request.

## 2.- You need to migrate a MySQL database with the least possible effort to Google Cloud. Which type of service would you use to accomplish this task? 

- a) **Cloud SQL** 
- b) BigQuery 
- c) Firestore 
- d) Bigtable 

    Explanation: Cloud SQL is a Google Cloud solution that allows us to create MySQL, PostgreSQL, and SQL Server instances.

## 3.- Your current solution receives messages on a publisher/subscriber (pub/sub) topic at a frequency in which the subscriber does not have real-time processing capacity. Which type of subscription would you use to avoid processing problems due to high frequency? 

- a) Static 
- b) Push 
- c) **Pull**
- d) Automatic 

    Explanation: A pull subscription allows us to obtain messages from a topic at the frequency we deem convenient, in order to be able to control high-frequency message scenarios without the subscriber collapsing.

    ### Types of subscriptions
    When you create a subscription, you must specify the type of message delivery. Pub/Sub offers two types of message delivery that corresponds to the following two types of subscriptions. Each type of subscription is described in brief in later sections of this document.
        - Pull subscription
        - Push subscription
    You can update the type of subscription at any time.

## 4.- Your current solution receives messages in a pub/sub topic, but the webhook that you have programmed to receive these messages does not allow the installation of external dependencies. Which type of subscription would you use to receive these messages with the aforementioned limitations? 

- a) Static 
- b) **Push** 
- c) Pull 
- d) Automatic 

    Explanation: A push-type subscription allows us to make calls to webhooks from Pub/Sub without the need to configure dependencies on the subscriber.

## 5.- We need to program within our application "a query" to Firestore that "mixes fairness and inequality operators". Which action do we need to perform within Firestore to allow this query? 

- a) **Composite index**
- b) Materialized views
- c) Document partition
- d) Split collections

    Explanation: When we have a query in Firestore that requires mixing fairness and inequality operators, it is necessary to create a composite index for these values; otherwise, Firestore will indicate an error.

    [TUTORIAL](https://www.youtube.com/watch?v=Ofux_4c94FI)