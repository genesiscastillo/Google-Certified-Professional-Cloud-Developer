# Managing APIs on GCP 

## 1.- How can we document an API so that it is understood by the various API management services? 

- a) Through HyperText Markup Language (HTML) 
- b) **Through the OpenAPI Specification (OAS)**
- c) Through LaTeX 
- d) Through Google Docs 

Open APi Specification [https://en.wikipedia.org/wiki/OpenAPI_Specification]

## 2.- Which component is it necessary to implement in our solutions to use Cloud Endpoints? 

- a) A storage service 
- b) **An Extensible Service Proxy (ESP)**
- c) A router 
- d) A computer service 

Explanation: An ESP allows calls to be intercepted before they reach our application, and thus they can be validated according to the rules defined in the documentation of our API through the OAS.

ESP [https://cloud.google.com/endpoints/docs/openapi/specify-proxy-startup-options]

```yaml
containers:
- name: esp
  image: gcr.io/endpoints-release/endpoints-runtime:1
  args: [
    "--http_port=8081",
    "--backend=127.0.0.1:8080",
    "--service=rtl-fal-corp-esup-fim-api-inventory-svc",
    "--rollout_strategy=managed",
    "--service_account_key=/etc/json/sa_esp_service.json"
  ]
```

## 3.- How can we protect calls to a service with Apigee? 

- a) **By verifying an API key in the PreFlow policy** 
- b) By configuring a reverse proxy
- c) By installing a virtual host 
- d) By restricting headers 

Explanation: The PreFlow flow configuration in Apigee allows us to apply policies before the request reaches our API.

  [TUTORIAL :: API Keys](https://docs.apigee.com/api-platform/security/api-keys)

## 4.- Which of these solutions allows users to create, secure, and monitor APIs in a serverless way? 

- a) Cloud Endpoints 
- b) **API Gateway** 
- c) Apigee
- d) API Management 

Explanation: API Gateway is a Google Cloud solution that allows us to execute the aforementioned tasks in a serverless way.

  [TUTORIAL GCP API Gateway](https://www.youtube.com/watch?v=KeSD76RDllk)

  * Apigee uses GCP services: Provides identity management, logging, analytics, metrics, and project management functions.
  * What is Apigee [https://cloud.google.com/apigee/docs/api-platform/get-started/what-apigee]

## 5.- Which HTTP verbs can we find in a REpresentational State Transfer (REST) API? 

- a) **GET, POST, PUT, and DELETE** 
- b) GET, READ, CREATE, and UPDATE 
- c) CLEAN, UPDATE, RESET, and DELETE 
- d) CLOSE, OPEN, READ, and DELETE

    __HTTP verbs__
    
    Si realizamos CRUD, debemos utilizar los HTTP verbs de forma adecuada para cuidar la semántica.
    **GET**: Obtener datos. Ej: GET /v1/empleados/1234
    **PUT**: Actualizar datos. Ej: PUT /v1/empleados/1234
    **POST**: Crear un nuevo recurso. Ej: POST /v1/empleados
    **DELETE**: Borrar el recurso. Ej: DELETE /v1/empleados/1234
    **¿PATCH?**: Para actualizar ciertos datos