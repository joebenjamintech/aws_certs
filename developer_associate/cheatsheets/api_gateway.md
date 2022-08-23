# api gateway

- a solution for creating secure APIs in your cloud environments at any scale
- create APIs that act as a front door for applications to access data, business logic, or functionality from back-end services
- throttles api endpoints at 10,000 requests per second (can be increased via service request through AWS support)
- **stages** allow you to have multiple published versions of your API e.g. prod, staging, QA
- each stage has an **invoke url** which is the endpoint you use to interact with your API
- you can use a custom domain for your invoke url
- you need to publish your api via deploy - you choose which stage you want to publish your api
- resources are your URLs e.g. projects
- resources can have child resources e.g. /projects/-id-edit
- you defined multiple methods on your resources EG. GET, POST, DELETE
- CORS issues are common with API gateway, CORS can be enabled on all or individual endpoints
- caching improves latency and reduces the amount of calls made to your endpoint
- same origin policies help to prevent XSS attacks
- same origin policies ignore tools like postman or curl
- CORS is always enforced by the client
- you can require authorization to your API via AWS cognito or a custom lambda
