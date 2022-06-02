# Using Cloud Functions and GAE

## 1.- With which of these services can Cloud Functions be integrated to receive events? 

- a) **Cloud Storage, Pub/Sub, and Firestore**
- b) GCE, Filestore, and Cloud Storage
- c) GKE, Cloud Run, and Cloud Storage 
- d) GAE, GCE, and Cloud Run


### [Events](https://cloud.google.com/functions/docs/concepts/events-triggers)

Events are things that happen within your cloud environment that you might want to take action on. These might be changes to data in a database, files added to a storage system, or a new virtual machine instance being created. Currently, Cloud Functions supports events from the following providers:

- HTTP
- Cloud Storage
- Cloud Pub/Sub
- Cloud Firestore
- Firebase (Realtime Database, Storage, Analytics, Auth)
- Cloud Logging—forward log entries to a Pub/Sub topic by creating a sink. You can then trigger the function.

---

## 2.- What kind of event is received in Cloud Functions when a new object is created in a Cloud Storage bucket? 

- a) **google.storage.object.finalize** 
- b) google.storage.object.delete 
- c) google.storage.object.archive 
- d) google.storage.object.metadataUpdate


[Triggers](https://cloud.google.com/functions/docs/calling/storage)

### Object Finalize
Trigger type value: **google.storage.object.finalize**
This event is sent when a new object is created (or an existing object is overwritten, and a new generation of that object is created) in the bucket.

### Object Delete
Trigger type value: **google.storage.object.delete**
This event is sent when an object is permanently deleted. Depending on the object versioning setting for a bucket this means:
- For versioning buckets, this is only sent when a version is permanently deleted (but not when an object is archived).
- For non-versioning buckets, this is sent when an object is deleted or overwritten.

### Object Archive
Trigger type value: **google.storage.object.archive**
This event is sent when a live version of an object is archived or deleted.
This event is only sent for versioning buckets.

### Object Metadata Update
Trigger type value: **google.storage.object.metadataUpdate**
This event is sent when the metadata of an existing object changes.

---
## 3.- What precaution should be taken when making asynchronous calls within a Cloud Functions application? 

- a) Make calls within the same project. 
- b) Wait for the call to finish and return a termination notice to the Cloud Functions application through promises. 
- c) Do not make more than two asynchronous calls in a single Cloud Functions application. 
- d) Do not make fewer than two asynchronous calls in a single Cloud Functions application. 

---
## 4.- Which kind of environments are there for GAE? 

- a) Standard and flexible 
- b) Standard and scalable 
- c) Flexible and regional 
- d) Flexible and scalable 

---
## 5.- If we need to test a functionality in production without impacting all our users, which of the following functionalities can we use? 

- a) HyperText Transfer Protocol (HTTP) functions with Cloud Functions
- b) Background functions with Cloud Functions 
- c) Call in/call out with GAE 
- d) Traffic splitting with GAE


