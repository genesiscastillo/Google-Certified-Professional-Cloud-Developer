# Google Cloud Platform (GCP) developer fundamentals

## 1.- As a developer, you have been tasked with transforming an application to high availability. Which factor should you consider to meet the requested objective? 

- a) Make sure that the application has at least two instances in the same organization.
- b) Make sure that the application has at least two instances in the same project. 
- c) Make sure that the application has at least two instances in the same zone. 
- d) **Make sure that the application has at least two instances in two different zones.**

    Explanation: Having a solution in a minimum of two zones allows our solution to continue working if the other zone is unavailable.

---
## 2.- Which of the following Google Cloud services is considered a Platform as a Service (PaaS) offering? 

- a) Google App Engine (GAE) 
- b) **Google Compute Engine (GCE)** 
- c) Google Kubernetes Engine (GKE)
- d) Cloud Functions 

    Explanation: GAE was one of the first products offered by Google Cloud and corresponds to a PaaS-type solution.
---
## 3.- How can we reduce latency when accessing our application data? 

- a) By increasing the number of instances of our application 
- b) **By applying a caching strategy in our application**   <--- MemoryStore
- c) By increasing the central processing unit (CPU) and random-access memory (RAM) of our application 
- d) By increasing the storage space of our application 

    Explanation: Applying a caching strategy to our application allows us to access a copy of the data source in a closer location, thus reducing latency in accessing this information.

---
## 4.- Which of the following Google Cloud services allows unlimited information storage? 

- a) Cloud SQL 
- b) GCE 
- c) **Google Cloud Storage** 
- d) Secret Manager 

---
## 5.- Which Google Cloud service allows you to decouple microservices in order to avoid the loss of information transmission in the event of an error?

- a) Firestore 
- b) **Pub/Sub**
- c) Memorystore 
- d) Secret Manager 

