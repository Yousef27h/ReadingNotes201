# APIs
1- What does REST stand for?

Representational state transfer

2- REST APIs are designed around a ____.

Resources

3- What is an identifer of a resource? Give an example.

a URI that uniquely identifies that resource.
```
https://adventure-works.com/orders/1
```

4- What are the most common HTTP verbs?

GET, POST, PUT, PATCH, and DELETE.

5- What should the URIs be based on?

URIs should be based on sources (nouns) not verbs (the operations on the resource).

6- Give an example of a good URI.

```
https://adventure-works.com/orders
```
7- What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

it means that such web APIs expose a large number of small resources. it's a bad thing, since the client server have to send multiple requests to to find all data it needs.

8- What status code does a successful GET request return?

returns HTTP status code 200 (OK) .

9- What status code does an unsuccessful GET request return?

return 404 (Not Found).

10- What status code does a successful POST request return?

it returns HTTP status code 201 (Created).

11- What status code does a successful DELETE request return?

the web server responds with HTTP status code 204.

## REST

REST is an architectural style for building distributed systems based on hupermedia. It is independent of any underlying protocol and is not necessarily tied to HTTP.
A primary advantage of REST over HTTP is that it uses open standards, and does not bind the implementation of the API or the client applications to any specific implementation.

Some of the main design principles of RESTful APIs using HTTP:

* REST APIs are designed around _resources_, which are any kind of object, data, or service that can be accessed by the client.
* A resource has an _identifier_, which is a URI that uniquely identifies that resource. 
* Clients interact with a service by exchanging _representations_ of resources.
* REST APIs use a uniform interface, which helps to decouple the client and service implementations. For REST APIs build on HTTP, the uniform interface includes using standard HTTP verbs to perform operations on resources (GET, POST, PUT, PATCH, and DELETE).
* REST APIs use a stateless request model. 


## Organize the API around resources

Focus on the business entities that the web API exposes. For example, in an e-commerce system, the primary entities might be customers and orders. Creating an order can be achieved by sending an HTTP POST request that contains the order information. The HTTP response indicates whether the order was placed successfully or not.

## Define operations in terms of HTTP methods

The common HTTP methods used by most RESTful web APIs are:

- __GET__ retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.
- __POST__ creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.
- __PUT__ either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.
- __PATCH__ performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.
- __DELETE__ removes the resource at the specified URI.


## Conform to HTTP semantics

### Media types
As mentioned earlier, clients and servers exchange representations of resources. For example, in a POST request, the request body contains a representation of the resource to create. In a GET request, the response body contains a representation of the fetched resource.
In the HTTP protocol, formats are specified through the use of media types, also called MIME types. For non-binary data, most web APIs support JSON (media type = application/json) and possibly XML (media type = application/xml).

### GET methods
A successful GET method typically returns HTTP status code 200 (OK). If the resource cannot be found, the method should return 404 (Not Found).
### POST methods

If a POST method creates a new resource, it returns HTTP status code 201 (Created). The URI of the new resource is included in the Location header of the response. The response body contains a representation of the resource.
If the method does some processing but does not create a new resource, the method can return HTTP status code 200 and include the result of the operation in the response body. Alternatively, if there is no result to return, the method can return HTTP status code 204 (No Content) with no response body.

### PUT methods

If a PUT method creates a new resource, it returns HTTP status code 201 (Created), as with a POST method. If the method updates an existing resource, it returns either 200 (OK) or 204 (No Content). In some cases, it might not be possible to update an existing resource. In that case, consider returning HTTP status code 409 (Conflict).

### PATCH methods

With a PATCH request, the client sends a set of updates to an existing resource, in the form of a patch document. The server processes the patch document to perform the update. The patch document doesn't describe the whole resource, only a set of changes to apply. The specification for the PATCH method (RFC 5789) doesn't define a particular format for patch documents. The format must be inferred from the media type in the request.

### DELETE methods

If the delete operation is successful, the web server should respond with HTTP status code 204, indicating that the process has been successfully handled, but that the response body contains no further information. If the resource doesn't exist, the web server can return HTTP 404 (Not Found).

