# CRUD

--------------

### Responses are grouped in five classes:
Informational responses (100–199) Successful responses (200–299) Redirects (300–399) Client errors (400–499) Server errors (500–599)

--------------

### What is a status code 202?

202 Accepted response status code indicates that the request has been accepted for processing, but the processing has not been completed

--------------
### What is a status code 308?

Permanent Redirect : redirect status response code indicates that the resource requested has been definitively moved to the URL given by the Location headers. A browser redirects to this page and search engines update their links to the resource (in 'SEO-speak', it is said that the 'link-juice' is sent to the new URL .

--------------
###  What code would you use if an update didn’t return data to a client?

204 No Content

--------------
###  What code would you use if a resource used to exist but no longer does?

410 Gone

### What is the ‘Forbidden’ status code?

403 Forbidden: The client has authorized , but still has no permissions to access the resource.

--------------

### Why do we need to pull our MongoDB database string out of our server and put it into our .env?

because when we gonna deploy the work on other place will not use the localhost

--------------

### What is middleware?

Middleware is software that provides common services and capabilities to applications outside of what’s offered by the operating system. Data management, application services, messaging, authentication, and API management are all commonly handled by middleware.

--------------


### What does app.use(express.json()) do?

to recognize the incoming Request Object as a JSON Object

--------------


### What does the /:id mean in a route?

Route parameters are named URL segments

--------------


### What is the difference between PUT and PATCH?

The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resourc

--------------


### How do you make a defalut value in a schema?

````
const subscruibedSchema = new mongoose.Schema({
    name:{

    },
    subscribe:{

    }
});
````

--------------


###  hat does a 500 error status code mean?

Internal Server Error server error response code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request. This error response is a generic "catch-all" response

--------------


###  What is the difference between a status 200 and a status 201?

The 200 status code is by far the most common returned. It means, simply, that the request was received and understood and is being processed. A 201 status code indicates that a request was successful and as a result, a resource has been created (for example a new page).

--------------



