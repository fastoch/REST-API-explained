REST APIs are **ubiquitous** in modern software, powering everything from weather apps to social media feeds.  

src = https://www.ibm.com/think/topics/rest-apis

# What is a REST API? 

A REST API is an application programming **interface** (API) that conforms to the design principles of the **representational state transfer** (REST) 
architectural style, a style used to connect distributed hypermedia systems. REST APIs are sometimes referred to as **RESTful** APIs or RESTful web APIs.  

REST APIs provide a lightweight way to build web APIs, and are commonly used to **facilitate data exchange** between applications, web services and databases, 
and to connect components in **microservices** architectures.  

# The 6 REST design principles 

At the most basic level, an API is a mechanism that enables an application or service to access a resource within another application, service or database.  

The application or service that accesses resources is the **client**, and the application or service that contains the resource is the **server**.  

Some APIs, such as SOAP or XML-RPC, impose a strict framework on developers.  
But developers can develop REST APIs using virtually any programming language and support a variety of data formats.  
The only requirement is that they align to the following six REST design principles, also known as **architectural constraints**.

## 1. Uniform interface

All API requests for the same resource should look the same, no matter where the request comes from.  
The REST API should ensure that the same piece of data, such as the name or email address of a user, belongs to only one uniform resource identifier (URI).  
Resources shouldn’t be too large but should contain every piece of information that the client might need.

## 2. Client-server decoupling

In REST API design, client and server applications must be completely **independent of each other**.  
The only information that the client application should know is the URI of the requested resource; it can't interact with the server application in any other ways.  
Similarly, a server application shouldn't modify the client application other than passing it the requested data via HTTP. 

## 3. Statelessness

REST APIs are **stateless**, meaning that each request needs to include all the information necessary for processing it.  
In other words, REST APIs do not require any server-side sessions. Server applications aren’t allowed to store any data related to a client request.

## 4. 

## 5. 

## 6. 

# How does a REST API work?

A REST API works by allowing a client, such as a web or mobile application, to communicate with a server using standard HTTP methods to interact with resources identified by URLs.  

The client sends HTTP requests (like GET, POST, PUT, DELETE) to manipulate resources, and the server replies with HTTP responses containing data or status information, usually in JSON format.  

## Client-Server Architecture

The client (user-facing app) and server (where data lives) operate **independently**, communicating only through the API's **interface**

## Statelessness

Each request from the client to the server must contain **all information needed** for fulfillment; **the server does not store client session state between requests**.

## Resource Orientation

Everything managed by the API is treated as a resource (such as a user, product, or document), each with a unique URI. 

## HTTP Methods

- **GET**: Retrieve data about a resource.
- **POST**: Create a new resource.
- **PUT**: Update an entire resource.
- **PATCH**: Partially update an existing resource.
- **DELETE**: Remove a resource

## Basic Example of REST API interaction

- The client sends a request, such as GET /api/users/1234, to fetch information about the user with id 1234.
- The server processes the request, accesses the data, and sends a response (usually in JSON).
- The client receives the response and uses it as needed (e.g., displaying user info)

