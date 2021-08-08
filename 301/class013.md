**In your own words, describe what each group of status code represents:**
100’s = informational status codes; they  tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client.

200’s =  the success codes. They tell the client that its request was accepted. 

300’s =  redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore.

400’s = the client error codes. They are all about invalid requests a client sent to a server. 

500’s = the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. 

**What is a status code 202?**

In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.

**What is a status code 308?**

08 Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

**What code would you use if an update didn’t return data to a client?**

204 No Content 

**What code would you use if a resource used to exist but no longer does?**

410 Gone - This is like 404 but we know that the resource existed in the past, but it got deleted or somehow moved, and we don’t know where.

**What is the ‘Forbidden’ status code?**

403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.






**Why do we need to pull our MongoDB database string out of our server and put it into our .env?**

because it is private information and we do not want to push it to gethub

**What is middleware?**

Middleware is software that provides common services and capabilities to applications outside of what's offered by the operating system.

**What does app.use(express.json()) do?**

xpress. json() is a method inbuilt in express to recognize the incoming Request Object as a JSON Object. This method is called as a middleware in your application using the code: app

**What does the /:id mean in a route?**

Route parameters are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys

**What is the difference beween PUT and PATCH?**

The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.

**How do you make a defalut value in a schema?**

You can define a default with a function or a value

**What does a 500 error status code mean?**

500 Internal Server Error server error response code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request.

**What is the difference between a status 200 and a status 201?**

**The 200 status code**  means that the request was received and understood and is being processed.
**A 201 status code** indicates that a request was successful and as a result, a resource has been created The request is identified by either a Location header field in the response or, if no Location field is received, by the effective request URI.
