# Application modernization using Google Cloud

## 1.- Which commands can we use with the Google Cloud service development kit (SDK)?
- a) npm, gcloud, and mvn 
- b) gcloud, npm, and bq 
- c) **gcloud, bq, and gsutil**
- d) gsutil, mvn, and gcloud 

### gcloud components
The **gcloud components** command group lets you control which tools are installed in the Google Cloud CLI. It can be used to install, update and remove components of the Google Cloud CLI, ensuring a lean, up-to-date installation.
**gcloud components** regularly checks whether updates are available for the tools you already have installed, and gives you the opportunity to upgrade to the latest version.

Certain components have dependencies. **gcloud components** will install any dependencies, and during removal, any dependant components will be uninstalled automatically.

| Descriptions components                              | commands                 |
|------------------------------------------------------|--------------------------|
| Cloud Firestore Emulator                             | cloud-firestore-emulator |
| Cloud Storage Command Line Tool                      | gsutil                   |
| Google Cloud CLI Core Libraries                      | core                     |
| gcloud Alpha Commands                                | alpha                    |
| gcloud Beta Commands                                 | beta                     |
| App Engine Go Extensions                             | app-engine-go            |
| Appctl                                               | appctl                   |
| Cloud Datalab Command Line Tool                      | datalab                  |
| Cloud Datastore Emulator                             | cloud-datastore-emulator |
| Cloud Run Proxy                                      | cloud-run-proxy          |
| Cloud SQL Proxy                                      | cloud_sql_proxy          |
| Google Container Registry's Docker credential helper | docker-credential-gcr    |
| Minikube                                             | minikube                 |
| Skaffold                                             | skaffold                 |
| anthos-auth                                          | anthos-auth              |
| config-connector                                     | config-connector         |
| gcloud app Java Extensions                           | app-engine-java          |
| gcloud app PHP Extensions                            | app-engine-php           |
| gcloud app Python Extensions                         | app-engine-python        |
| gcloud app Python Extensions (Extra Libraries)       | app-engine-python-extras |
| kubectl                                              | kubectl                  |
| kubectl-oidc                                         | kubectl-oidc             |
| pkg                                                  | pkg                      |
| BigQuery Command Line Tool                           | bq                       |
| Cloud Bigtable Command Line Tool                     | cbt                      |
| Cloud Bigtable Emulator                              | bigtable                 |
| Cloud Pub/Sub Emulator                               | pubsub-emulator          |



---

## 2.- What kind of test verifies that a particular component is performing a task correctly? 
 - a) **Unit test**
 - b) Integration test 
 - c) Load test 
 - d) End-to-end (E2E) test

### The different types of tests

#### Unit tests
Unit tests are very low level, close to the source of your application. They consist in testing individual methods and functions of the classes, components or modules used by your software. Unit tests are in general quite cheap to automate and can be run very quickly by a continuous integration server.

#### Integration tests
Integration tests verify that different modules or services used by your application work well together. For example, it can be testing the interaction with the database or making sure that microservices work together as expected. These types of tests are more expensive to run as they require multiple parts of the application to be up and running.

#### Functional tests
Functional tests focus on the business requirements of an application. They only verify the output of an action and do not check the intermediate states of the system when performing that action.
There is sometimes a confusion between integration tests and functional tests as they both require multiple components to interact with each other. The difference is that an integration test may simply verify that you can query the database while a functional test would expect to get a specific value from the database as defined by the product requirements.

#### End-to-end tests
End-to-end testing replicates a user behavior with the software in a complete application environment. It verifies that various user flows work as expected and can be as simple as loading a web page or logging in or much more complex scenarios verifying email notifications, online payments, etc...
End-to-end tests are very useful, but they're expensive to perform and can be hard to maintain when they're automated. It is recommended to have a few key end-to-end tests and rely more on lower level types of testing (unit and integration tests) to be able to quickly identify breaking changes.

---

## 3.- Which Google Cloud solution can we use to store the source code of our applications?

- a) Google Container Registry 
- b) Developer Tools 
- c) Cloud Build 
- d) **Cloud Source Repositories**

**[Cloud Source Repositories](https://cloud.google.com/source-repositories/docs/create-code-repository#:~:text=Cloud%20Source%20Repositories%20are%20private,version%20control%20for%20your%20code.)** are private Git repositories hosted on Google Cloud. These repositories let you develop and deploy an app or service in a space that provides collaboration and version control for your code.

---

## 4.- Which Google Cloud solution can we use to create a Continuous Integration/Continuous Delivery (CI/CD) stream for our applications?

- a) Developer Tools 
- b) **Cloud Build**
- c) Google Cloud SDK 
- d) Cloud Composer


**Cloud Build** is a service that executes your builds on Google Cloud.

**Cloud Build** can import source code from a variety of repositories or cloud storage spaces, execute a build to your specifications, and produce artifacts such as Docker containers or Java archives.

[TUTORIAL](https://www.youtube.com/watch?v=rWEd9CYw9_s)

---
### 5.- Which Google Cloud solution can we use to store the container images of our applications?

- a) **Container Registry**
- b) Secret Manager 
- c) GKE 
- d) GCE

**Container Registry** A private container image registry that supports Docker Image Manifest V2 and OCI image formats. It provides a subset of Artifact Registry features.

[TUTORIAL](https://www.youtube.com/watch?v=_XAk5T_4-O0)
---
