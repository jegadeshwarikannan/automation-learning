#### API:

> API - Application Programming Interface

An API exposes functionality or data of a service so other programs can interact with it.
Developer write programs to consume it

>  **Why API?** Reduced complexity

> **How does an API work** -> Documentation

##### Components of a request:

There are 4 component to an HTTP request:

- URL
- Method
- Header
- Body (Optional)
##### 1. URL 

	Unique location for a resource on the web (page,img,pdf etc...)

![Automation](../assets/Pasted%20image%2020260927001159.png.png)

##### 2. Method

Describes the actions to be performed at the given URL

2 Common methods of a HTTP Request are:
- `GET` → retrieve data
- `POST` → send/create data
- `PUT` → replace/update a resource
- `PATCH` → partially update a resource
- `DELETE` → delete a resource

##### 3. Header
Gives more detail (context) to the request
Headers provide additional metadata/context about the request or response.

Common Info in headers:
- Location 
- Language
- Device Type

>Example Header:
>Accept: application/json -> tells the server it would like the response in the JSON format

> Authorization: Bearer <token>
> Content-Type: application/json
> Accept: application/json

##### 4. Body
Optional
Data sent to the server, commonly used with POST, PUT, and PATCH.
##### 5. Credentials
How we let the application know that we are allowed to make the given request
Authentication tells the server who/what is making the request and whether it is allowed to access the resource.

2 main ways of authentication:
- Query parameter: ?api_key=xxx_xxx_xxx
- Header: Authorization: Bearer xxx_xxx_xxx

##### Components of a Response:

The 3 main components of a HTTP response are 
- Status code
- Header
- Body

##### 1. Status Code
This is a 3 digit number that indicates whether the request was successful or not

Some common status codes are,
- **200** : OK
- **401** : Unauthorized
- **404** : Not Found
- **500** : Internal Server Error
##### 2. Header

Gives more context (detail)

Some common response headers:
- Content - length
- Content - Type
- Expires

##### 3. Body
The actual data returned
They can be of different types as mentioned in the header
- HTML
- JSON
- Data


#### Webhooks - API^-1

Reverse API
A **webhook is a way for one application to automatically send data to another application when an event happens.**

Think of it as:

**Event happens → App sends data → Your workflow starts**

|API|Webhook|
|---|---|
|You request data/action|Another system sends you data|
|Usually request-driven|Event-driven|
|Your app initiates the request|External app initiates the request|
|`Your app → API`|`External app → Your webhook`|