# Class 12
## Status Codes Based On REST Methods

### In your own words, describe what each group of status code represents:

100's =  tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client

200's = They tell the client that its request was accepted.

300's = They tell the client that the resource they are requesting isn’t available at the expected location anymore.

400's = They are all about invalid requests a client sent to a server.

500's = These are the server error codes.
### What is a status code 202?
This code tells the client that the request was valid, but its processing will finish sometime in the future

### What is a status code 308?
his tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one
### What code would you use if an update didn't return data to a client?
204 No Content 

### What code would you use if a resource used to exist but no longer does?
410 Gone
### What is the 'Forbidden' status code?
The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource. (308)

---

## Build A REST API With Node.js, Express, & MongoDB - Quick -

### Why do we need to pull our MongoDB database string out of our server and put it into our .env?
 because the link as senstive information
### What is middleware?
   software that acts as a bridge between an operating system or database and applications, especially on a network.
### What does app.use(express.json()) do?
to make the server except json
### What does the /:id mean in a route?
 request value and can acsses to it
### What is the difference between PUT and PATCH?
path update what user pass / put update all the user at once  
### How do you make a default value in a schema?
 write deafult: var.now inside the schema
### What does a 500 error status code mean?
there is an error on your server

### What is the difference between a status 200 and a status 201?
201 syccess to make an object
200 everything was successful