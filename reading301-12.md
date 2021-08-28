# [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

### In your own words, describe what each group of status code represents:
* 100’s =These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. Like using a different protocol or telling the client that its request will fail before they start sending the body.


* 200’s =These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.


* 300’s =These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. This can have multiple reasons, be temporary or permanent, but the client has to issue a request to the new location.


* 400’s =These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication, etc. A client is sending incorrect input and should confirm the input parameters are correct before retrying the request.


* 500’s =These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. These errors can be temporary or permanent. Usually it’s best for the client to retry the same request.



What is a status code 202?
Accepted . request has met all validation requirements at the time of sending.


What is a status code 308?
*  Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.

What code would you use if an update didn’t return data to a client?
* 204 No Content

What code would you use if a resource used to exist but no longer does?
* 410 gone

What is the ‘Forbidden’ status code?
* The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

## [Build A REST API With Node.js, Express, & MongoDB](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

### Why do we need to pull our MongoDB database string out of our server and put it into our .env?
*  beacuse it is sensitve to shar the url link for our data base. 
### What is middleware?
* code that runs before the final route call back. They are in the middle of the beginning of the route and the callback function.
### What does app.use(express.json()) do?
* Returns middleware that parses both json and urlencoded. The options are passed to both middleware.
### What does the /:id mean in a route?
Route parameters are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys.
* 
### What is the difference beween PUT and PATCH?
* The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.
### How do you make a defalut value in a schema?
>const schema = new Schema({
  name: String,
  role: { type: String, default: "guitarist" },
});
### What does a 500 error status code mean?
* This error response is a generic “catch-all” response. 500 Internal Server Error server error response code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request.
### What is the difference between a status 200 and a status 201?
* that the request was received and understood and is being processed. A 201 status code indicates that a request was successful and as a result, a resource has been created .