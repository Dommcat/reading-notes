# 301 Reading Notes

## Class 12 Summary: This class reading is about CRUD

In your own words, describe what each group of status code represents:

100’s = Informational between server and client
200’s = Sucess codes
300’s = Redirect/requesting isn’t available
400’s = Client error codes/invalid requests
500’s = Server error codes

What is a status code 202?
202 Accepted - Often used for asynchronous processing. 

What is a status code 308?
308 Permanent Redirect

What code would you use if an update didn’t return data to a client?
204 No Content - A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.

What code would you use if a resource used to exist but no longer does?
308 Permanent Redirect - This would be the right code if we know that a resource has moved to a different URL and we can tell the client about it.
307 Temporary Redirect - Same as 308, but we don’t know if the resource will be back on the original URL or another different URL in the future.


What is the ‘Forbidden’ status code?
403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.


## MongoDB

Why do we need to pull our MongoDB database string out of our server and put it into our .env?


What is middleware?


What does app.use(express.json()) do?
create express library

What does the /:id mean in a route?


What is the difference between PUT and PATCH?


How do you make a default value in a schema?


What does a 500 error status code mean?


What is the difference between a status 200 and a status 201?


## Things I want to know more about