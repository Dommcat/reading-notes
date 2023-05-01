# 401 Advanced Python: Class 31 Reading Notes

## Summary: This class reading is about: Django REST Framework & Docker


 - Virtual environments are used to isolate Python software packages locally and can only isolate Python packages

**Qp**:What are the key components of a Docker container, and how do they help streamline the development and deployment of applications?


**A**: Docker containers have four key components: 

Key Components:

- Docker Image: snapshot of application and dependencies
- Docker Registry: centralized location for storing Docker images
- Docker Engine: runtime environment for running Docker containers
- Dockerfile: specifies instructions to build a Docker image

Benefits:

- Consistent application performance across different environments
- Standardized deployment process
- Reduced risk of configuration errors
- Easy scaling of applications
- Streamlined development and deployment process
- Allows developers to focus on writing and testing code.

**Qp**:Describe the primary steps involved in building a library website using Django, including essential components like models, views, and templates.

**A**:
- Define Models: Define models for books, authors, users, and borrowing records.
- Create Views: Create views to handle requests and display information, such as a list of books or a search form.
- Design Templates: Design templates to render pages and display dynamic content.
- Connect Views and Templates: Connect views and templates using URLs to map specific views to URL patterns.
- Implement Authentication and Authorization: Implement authentication and authorization to secure the website and ensure users  can only access authorized content.
- Test and Deploy: Test the website using Django's built-in testing tools, then deploy it to a production server for public use.


**Qp**:explain the primary differences between Django and Django REST framework?

**A**:key differences between Django and Django REST framework
 -Purpose: Django is a full-stack web framework for building server-rendered web applications, while DRF is a framework for building web APIs.
- URL routing: Django uses a separate urls.py file for each app, while DRF uses a single urls.py file for the entire project.
- Serialization: DRF provides serializers for converting Python objects to JSON, XML, or other formats, which Django does not have built-in.
- Response types: Django renders HTML templates, while DRF primarily returns JSON responses for API requests.
- Authentication: DRF includes built-in authentication classes, while Django requires custom authentication implementations.
- Views: Django provides generic views, while DRF provides views for handling API requests and generating JSON responses.
- Documentation: DRF includes built-in documentation tools, while Django does not have this functionality.



## Sources:

ChatGPT 

https://asgi.readthedocs.io/en/latest/specs/main.html

https://wsvincent.com/beginners-guide-to-docker/

https://djangoforapis.com/library-website-and-api/


## Things I want to know more about
Virtual Computers 

https://en.wikipedia.org/wiki/Virtualization
