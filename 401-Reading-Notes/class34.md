# 401 Advanced Python: Class 34 Reading Notes

## Summary: This class reading is about: API Deployment


What are the key principles to follow when organizing and configuring Django settings for a project, according to the “Django Settings Best Practices” reading?

- Key principles for organizing and configuring Django settings include keeping settings modular, using environment variables, and using separate settings files for each environment.
- Use environment variables to store sensitive or environment-specific settings, and avoid storing sensitive data in version control.
- Follow naming conventions and provide default values for settings variables.
- Following these principles helps to maintain a clean, organized, and secure Django project with well-structured settings that can be easily managed and modified across different environments.


What is the purpose of Cross-Origin Resource Sharing (CORS) in web applications, and how can it be implemented and configured in a Django project to control access to resources?

- Cross-Origin Resource Sharing (CORS) is a security feature implemented in web browsers that controls access to resources on different domains.
- The purpose of CORS is to prevent web applications from making unauthorized requests to resources on other domains.
- CORS can be implemented and configured in a Django project using the `django-cors-headers` package, which allows developers to specify which domains are allowed to access resources in the project.

Details:

- The purpose of CORS is to prevent web applications from making unauthorized requests to resources on other domains. It is a security feature implemented in web browsers that controls access to resources on different domains.
- Without CORS, web applications can make cross-domain requests, which can be exploited by attackers to steal data or perform unauthorized actions.
- CORS works by requiring web applications to specify which domains are allowed to access resources on the server.
- CORS can be implemented and configured in a Django project using the `django-cors-headers` package, which provides middleware to add CORS headers to HTTP responses.
- To use `django-cors-headers`, install the package and add the middleware to the project's settings file.
- In the settings file, specify which domains are allowed to access resources using the `CORS_ORIGIN_WHITELIST` setting.
- Additional settings can be used to customize the behavior of `django-cors-headers`, such as specifying which HTTP methods are allowed, adding custom headers, and controlling whether cookies can be sent with cross-origin requests.
- By implementing and configuring CORS in a Django project using `django-cors-headers`, developers can control access to resources and prevent unauthorized cross-domain requests, helping to maintain the security of the application.


## Re/Sources:

Chatgpt

https://whitenoise.readthedocs.io/en/stable/

https://en.m.wikipedia.org/wiki/Cross-origin_resource_sharing

https://djangostars.com/blog/configuring-django-settings-best-practices/

## Things I want to know more about
naming conventions