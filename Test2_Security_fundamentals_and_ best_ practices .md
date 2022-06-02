# Security fundamentals and best practices 

## 1.- If we want to minimize the possibility that a part of our application executes unauthorized tasks, which principle should we apply in the configuration of the service accounts of our application? 

- a) Principle of least use of resources 
- b) **Principle of least privilege (POLP)** 
- c) Principle of isolation 
- d) Principle of escalation 

**The principle of least privilege (POLP)** is a computer security concept and practice that gives users limited access rights based on the tasks necessary to their job. POLP ensures only authorized users whose identity has been verified have the necessary permissions to execute jobs within certain systems, applications, data and other assets.

POLP is widely considered to be one of the most effective practices for strengthening the organization’s cybersecurity posture, in that it allows organizations to control and monitor network and data access.

---
## 2.- In which way can we give permissions to users and applications within Google Cloud for other components? 

- a) **Through Identity and Access Management (IAM)** 
- b) Through the administration manager 
- c) By using a username and password 
- d) Through certificates 

Google Cloud offers **Identity and Access Management (IAM)**, which lets you give more granular access to specific Google Cloud resources and prevents unwanted access to other resources. IAM lets you adopt the security principle of least privilege, so you grant only the necessary access to your resources.

IAM lets you control who (users) has what access (roles) to which resources by setting IAM policies, which grant specific roles that contain certain permissions.

---
## 3.- How is the hierarchy of resources composed within Google Cloud? 

- a) **Organization, folders, projects, and resources** 
- b) Resources, projects, folders, and organization 
- c) Folders, projects, organization, and resources 
- d) Resources, projects, folders, and folders 

[Resource hierarchy](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy)

![img](cloud-hierarchy.svg)

---
## 4.- How can I safely store my application credentials?

- a) Directly in the source code 
- b) In a relational database 
- c) In a non-relational database 
- d) **In Secret Manager** 

Secret Manager is a secure and convenient storage system for API keys, passwords, certificates, and other sensitive data. Secret Manager provides a central place and single source of truth to manage, access, and audit secrets across Google Cloud.

```bash
gcloud secrets create secret-id --replication-policy="automatic"

```

---
## 5.- What is the recommended way to authenticate with a service from an application in Google Cloud? 

- a) **Service account**
- b) Username and password 
- c) Application programming interface (API) key 
- d) Certificates


A service account is a special kind of account used by an application or compute workload, such as a Compute Engine virtual machine (VM) instance, rather than a person. Applications use service accounts to make authorized API calls, authorized as either the service account itself, or as Google Workspace or Cloud Identity users through domain-wide delegation.

For example, a service account can be attached to a Compute Engine VM, so that applications running on that VM can authenticate as the service account. In addition, the service account can be granted IAM roles that let it access resources. The service account is used as the identity of the application, and the service account's roles control which resources the application can access.

A service account is identified by its email address, which is unique to the account.
