# 401 Advanced Python: Class 33 Reading Notes

## Summary: This class reading is about: Authentication & Production Server


- JSON Web Tokens (JWTs) are a popular way to securely transmit data between parties as a JSON object.
- The primary purpose of JWTs is to provide a means of authentication and authorization.
- JWTs work by encoding data as a compact, URL-safe string that can be easily transmitted over the network.
- JWTs consist of three parts: a header, a payload, and a signature.
- The header contains metadata about the token, such as the signing algorithm used.
- The payload contains the claims, or statements about an entity (e.g., user ID, role, expiration time).
- The signature is used to verify that the message has not been tampered with.
- To encode a JWT, the header and payload are first Base64Url encoded and concatenated with a period separator.
- The resulting string is then signed using a secret key or public/private key pair.
- To decode a JWT, the signature is first verified to ensure the message has not been tampered with.
- The Base64Url encoded header and payload can then be decoded to reveal the claims about the entity.


How does JWT Authentication integrate with Django REST Framework to secure API endpoints/components


- JWT authentication can be used with Django REST Framework to secure API endpoints.
- DRF's built-in authentication classes do not include JWT authentication by default.
- Custom authentication views can be created to handle JWT authentication using PyJWT library to create and verify JWTs.
- PyJWT provides methods for encoding and decoding JWTs.
- A custom authentication view is created to verify the JWT included in the `Authorization` header of a request.
- The authentication view decodes and verifies the signature of the JWT and extracts user information from the payload.
- If the JWT is valid, DRF allows the request to proceed and the user information can be used to control access to the requested resource.
- If the JWT is invalid or missing, an error response is returned, indicating that the client is not authorized to access the requested resource.


Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?

- Django's `runserver` command is designed for development purposes and lacks important features required for production environments, such as security and performance optimizations.
- Production environments require a dedicated web server such as Apache or Nginx to host the Django application, along with additional security and performance optimizations.
- Other considerations for deploying a Django application include choosing a hosting provider, using a cloud-based hosting service, or using a containerization platform such as Docker to simplify the deployment process and manage application dependencies.
- Best practices for securing and optimizing the Django application should be followed, including using a production-ready web server, regularly updating the server software, and monitoring server performance and security.


## Re/Sources:

Chatgpt

https://www.youtube.com/watch?v=Fhcn2qx-4VQ

https://jwt.io/introduction/

https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html

https://vsupalov.com/django-runserver-in-production/

## Things I want to know more about

servers 



