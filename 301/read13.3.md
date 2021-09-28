# CRUD

![image](https://www.dorusomcutean.com/wp-content/uploads/2020/03/crud.jpg)

## Which HTTP Status Code to Use for Every CRUD App

When replying to our customers, the HTTP standard offers a number of status codes that we may utilize. Some APIs just utilize the most basic codes and build their own error signaling systems on top of them; others wish to use the entire HTTP code set to inform their customers about what's going on. This essay is for you if you fall into the latter category. For a clean API architecture, this article guides you through the different CRUD actions and which status codes you should use.

## HTTP Status Codes

A status code is a number in the HTTP response that is more than 100 but less than 600. The status's class is determined by the first digit. A rationale sentence is included with each status code. The sentence is for people to comprehend what happened, while the code is for automated recognition.

These two requirements must be followed by all status codes, including bespoke ones (yes the status codes are extensible).

## Status Classes

We can more easily discover problems if we know what class a status code belongs to.

- 100 - 199\
These are informative status codes that typically indicate the client that the header portion of the request has been received and that the server will attempt to fulfill the client's transmission request. For example, you might use an alternative protocol or inform the client that their request will fail before delivering the body.

- 200 - 299\
These are the keys to success. They inform the customer that their request has been granted. Asynchronous request processing (202), on the other hand, does not imply that the request was successfully processed; rather, it means that it fulfilled all validation criteria at the time of sending.

- 300 - 399\
This is a list of redirection codes. They inform the client that the requested resource is no longer accessible at the expected location. This might be for a variety of reasons, including temporary or permanent relocation, but the customer must submit a request to the new location.

- 400 - 499\
These are the error codes for clients. They're all about incorrect requests made to a server by a client. There are numerous reasons for this, including timeouts, incorrect URIs, and insufficient authentication. If a client sends erroneous data, the request should be retried after double-checking the input parameters.

- 500 - 599\
The server error codes are shown below. They frequently signal issues with overburdened servers or inaccessible servers behind proxies, but they can also be directly connected to client requests that cause server error exceptions. Temporary or permanent mistakes might occur. Retrying the same request is usually the best option for the customer.

## CRUD (Create, Read, Update, Delete)

### Creat

The POST method is commonly used to accomplish the create action. These endpoints are used to create new resources or access tokens in RESTful APIs.

### READ

The read action is used to obtain resource representations and is implemented using HTTP's GET method. Asynchronous replies aren't common since the reason for asynchronous processing is because the resource doesn't exist yet and must be generated, thus it's essentially a create action.

### UPDATE

An HTTP PUT or PATCH method can be used to do an update. The difference is in the amount of data sent to the backend by the client.

To update a resource, PUT needs the client to transmit the complete representation of the resource. (Place the new one in place of the old one.)

To update a resource, PATCH requires the client to only transmit portions of the representation. (In the previous version, add, edit, or delete these elements.)

### DELETE

The HTTP DELETE method can be used to perform the delete operation.

## API Changes

If our API is around for a long time, it will eventually change its structure. It's essential to prevent breaking changes, and the redirection class of status codes can assist because certain clients will automatically follow their Location header.
