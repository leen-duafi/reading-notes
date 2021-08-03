**What does REST stand for?**

Representational State Transfer

**REST APIs are designed around a ____.**

REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

**What is an identifer of a resource? Give an example.**

A resource has an identifier, which is a URI that uniquely identifies that resource

https://adventure-works.com/orders/1

**What are the most common HTTP verbs?**

he most common operations are GET, POST, PUT, PATCH, and DELETE.

**What should the URIs be based on?**

URIs should be based on nouns (the resource) and not verbs (the operations on the resource)

**Give an example of a good URI.**

* example.com/articles/3252
* example.com/articles/how+to+design+good+uri

**What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**

 a large number of small resources , bad thing 

**What status code does a successful GET request return?**

he body of the response message contains the details of the requested resource.

**What status code does an unsuccessful GET request return?**

A successful GET method typically returns HTTP status code 200 (OK). If the resource cannot be found, the method should return 404 (Not Found).

**What status code does a successful POST request return?**

* If the method does some processing but does not create a new resource ..... the method can return HTTP status code 200 and include the result of the operation in the response body.

* if there is no result to return,.......the method can return HTTP status code 204 (No Content) with no response body.

* If the client puts invalid data into the request, the server should return HTTP status code 400 (Bad Request). The response body can contain additional information about the error or a link to a URI that provides more details.

**What status code does a successful DELETE reque**

* If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content), indicating that the process has been successfully handled, but that the response body contains no further information.

* If the resource doesn't exist, the web server can return HTTP 404 (Not Found).