## Reading Notes Class 12

#### Status Codes Based On REST Methods

100’s = informational status codes - tells client request will fail before sending the body
200’s = success codes that mean request was accepted 
300’s = redirection codes - resources that have been requested aren't available
400’s = client error codes - invalid requests that caused by various reason
500’s =server error codes - problem with overwhelmed server or unreachable servers

1. What is a status code 202?
  - used for async processing. Creation from backend 
2. What is a status code 308?
  - permanent redirection to tell client to use different URL
3. What code would you use if an update didn’t return data to a client?
  - 204, tells client that updates didn't return data to client 
4. What code would you use if a resource used to exist but no longer does?
  - 410 is a resource that existed in the past, but got deleted
5What is the ‘Forbidden’ status code?
  - 403, client has authorization or doesn't need authorization. but has no permissions to access resource

#### Videos
###### Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
  - use to connect mongoDB with server
2. What is middleware?
  - code that runs when the server get a request but before it gets past to the route
3. What does app.use(express.json()) do?
  - allows code to be accpeted as a body or anything else
4. What does the /:id mean in a route?
  - gives access to whatever is passed in after first slash
5. What is the difference between PUT and PATCH?
  - only updates what the user passes rather than updating all the information which is what put does
6. How do you make a default value in a schema?
  - use default: define a value
7. What does a 500 error status code mean?
  - error on server, server/DB has an error which caused transaction not to work
8. What is the difference between a status 200 and a status 201?
  - 201 means it was successful AND you created something