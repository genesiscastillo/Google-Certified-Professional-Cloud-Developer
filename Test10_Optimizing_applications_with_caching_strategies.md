# Optimizing applications with caching strategies on GCP 

## 1.- Which kind of caching database can be implemented using Memorystore? 

- a) MongoDB 
- b) Bigtable 
- c) **Redis** 
- d) Firestore 

## 2.- You are asked to implement a caching strategy within existing code in Cloud Functions. Which action should you consider so that Cloud Functions can communicate with Memorystore? 

- a) **Serverless virtual private cloud (VPC) access**
- b) Firewall rules 
- c) Load balancer 
- d) Ingress 

    [Speed up your API on Cloud Run with Memorystore caching](https://www.youtube.com/watch?v=BjRAO51omQs)

## 3.- What are the benefits of implementing a caching strategy in your application? 

- a) Simplification of business logic 
- b) **Reduction of latency and use of resources**
- c) Reduction of the number of components to be used 
- d) Simplification of the solution architecture 

    [Working with GCP Memorystore](https://www.red-gate.com/simple-talk/blogs/working-with-gcp-memorystore/)

## 4.- In which of the following scenarios is the use of a caching strategy recommended?

- a) When the source data changes to a low frequency
- b) **When the source data changes to a high frequency**
- c) When transactional operations are carried out 
- d) When having up-to-date data is critical to the operation

## 5.- Which other benefits related to the availability of our services can the implementation of a caching strategy in our applications provide us? 

- a) Maintain an additional data source in case of the unavailability of a service. 
- b) Simplification of the use of resources. 
- c) Increase in computing speed. 
- d) Reduction in the use of RAM.

---
# [MemoryStore for Redis](https://cloud.google.com/memorystore/docs/redis/create-instance-gcloud)

    ### Crear y administrar instancias de Redis [DOC](https://cloud.google.com/memorystore/docs/redis/creating-managing-instances)

    #### Crea una instancia de Redis en una red de VPC

    ```bash
    gcloud redis instances create INSTANCE_ID --size=SIZE --region=REGION_ID
    ```

    #### Creating a Redis instance on a Shared VPC network from a service project

    ```bash
    gcloud redis instances create INSTANCE_ID --size=SIZE --region=REGION_ID --project=SERVICE_PROJECT_ID \
    --network=projects/HOST_PROJECT_ID/global/networks/HOST_NETWORK_NAME \
    --connect-mode=private-service-access
    ```

