### Modernizing Applications with Apigee X

### Overview



Google Cloud's Apigee API Platform can be used to modernize existing applications by adding new functionality to your existing APIs.

In this lab, you deploy a backend service on Cloud Run.   The backend service implements a REST API that stores and retrieves bank data (customers, accounts, ATMs, and transactions) in a Firestore database.   You create an Apigee API proxy that proxies the backend service.   You also create a shared flow that retrieves and caches content from an external service. You then call that shared flow from your API proxy and use JavaScript code to modify an API response.

### Objectives


- Deploy a backend service on Cloud Run  
- Proxy a backend service using an Apigee X proxy  
- Create a shared flow for functionality that can be used by multiple proxies  
- Store configuration data in a property set  
- Use a service callout policy to retrieve content from a service  
- Use cache policies to cache reusable information  
- Use JavaScript code to modify a response payload  

### Setup
Google Cloud 

### Task 1. Deploy a backend service on Cloud Run

In this task, you deploy a backend service on Cloud Run.

The service implements an API for SimpleBank. This API provides a simple representation of a bank, with customers, accounts, transactions, and ATMs. The SimpleBank service is built using Node.js with data stored in Firestore. The code is packaged in a Docker container, and this container is deployed to Cloud Run.







