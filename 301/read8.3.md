# APIs
![image](https://developers.giphy.com/branch/master/static/api-c99e353f761d318322c853c03ebcf21b.gif)

## RESTful web API design

The majority of current online apps provide APIs that clients may utilize to communicate with them. A well-designed web API should attempt to offer the following features:

- Independent of the platform. Regardless of how the API is built inside, any client should be able to call it. This necessitates the use of standard protocols and the establishment of a system through which the client and the web service can agree on the data format to be sent.

- The development of the service Client apps should not be allowed to evolve or add functionality to the web API. Existing client apps should continue to work without modification as the API evolves. All functionality should be discoverable by client programs so that they may take full use of it.

## What is REST?

Roy Fielding introduced Representational State Transfer (REST) as a design strategy for web services in 2000. REST is an architectural approach for creating hypermedia-based distributed systems. REST is not bound to HTTP and is independent of any underlying protocol. However, HTTP is the most popular application protocol for REST APIs, and this article concentrates on developing REST APIs using HTTP.

One of the main advantages of REST over HTTP is that it is based on open standards and does not tie the API or client applications to any particular implementation. Client applications can use any language or toolset that can produce HTTP requests and read HTTP replies, for example, a REST web service might be developed in ASP.NET.

The following are some of the most important design concepts for RESTful APIs that use HTTP:

- REST APIs are built around resources, which can be any type of object, data, or service that the client can access.

- A resource has an identifier, which is a URI that uniquely identifies that resource. For instance, the URI for a specific client order may be:

HTTP

https://adventure-works.com/orders/1

- Clients communicate with a service by exchanging resource representations. JSON is a popular interchange format for online APIs. A GET request to the URI given above, for example, may produce the following response body:

JSON

{"orderId":1,"orderValue":99.90,"productId":1,"quantity":1}.

- REST APIs utilize a standardized interface to assist decouple client and service implementations. The universal interface for REST APIs built on HTTP enables performing actions on resources using standard HTTP verbs. GET, POST, PUT, PATCH, and DELETE are the most frequent operations.

- A stateless request paradigm is used by REST APIs. Keeping transitory state information between requests is not possible since HTTP requests should be autonomous and can happen in any order. The resources themselves are the sole area where information is kept, and each request should be an atomic process. Because there is no need to maintain any affinity between clients and specific servers, this limitation allows web services to be very scalable. Any server can handle any client's request. Other variables, though, can limit scalability.

## Organize the API design around resources

Concentrate on the business entities exposed via the web API. Customers and orders, for example, may be the key entities in an e-commerce system. Sending an HTTP POST request with the order information can be used to create an order. The HTTP response code shows whether or not the order was successfully placed. Resource URIs should, if feasible, be based on nouns (the resource) rather than verbs (the operations on the resource).

It is not necessary for a resource to be based on a single physical data piece. An order resource, for example, may be implemented as several tables in a relational database but displayed to the client as a single object. Avoid making APIs that merely replicate a database's underlying structure. The goal of REST is to represent entities and the actions that may be performed on them by an application. The internal implementation should not be shown to a client.