# 401 Advanced Python: Class 29 Reading Notes

## Summary: This class reading is about: Django Custom User

Django Custom User is a feature in the Django web framework that allows developers to create their own user models, tailored to their specific application requirements. It provides flexibility and customization beyond the default Django User model, enabling developers to modify, add, or remove fields related to authentication, authorization, and user data management. This allows for a more personalized user experience and better security, while ensuring the application's long-term scalability and maintainability.


**Qp**: What are the key benefits of using a Django Custom User Model, and how does it differ from the default Django User Model?


**A**: Key benefits of using a Django Custom User Model include:

Flexibility: Custom User Models enable developers to add, modify, or remove fields according to the specific requirements of their applications, providing more control over user data management.
Customization: Developers can tailor authentication and authorization processes to suit their application's unique needs.
Improved Security: Customizing user models can enhance security by allowing the implementation of additional authentication measures and more granular user permissions.
Scalability: Custom User Models ensure long-term scalability by allowing developers to modify user-related aspects of the application without impacting existing functionality.
Maintainability: A Custom User Model allows for easier updates and maintenance, as the developer can make changes directly to the custom model without affecting the default Django User model.
The key differences between the Django Custom User Model and the default Django User Model are:

Fields: The default Django User model includes pre-defined fields such as username, first_name, last_name, email, password, etc. A Custom User Model allows developers to add, modify, or remove fields as needed.
Authentication: Custom User Models enable developers to implement unique authentication methods or use alternative identifiers (e.g., email address instead of a username).
Authorization: Custom User Models can include additional or customized permissions and group management to fit the application's requirements.
Adaptability: Custom User Models allow for adjustments to user-related features without disrupting the default Django User model, making it easier to adapt the application to changing requirements.






**Qp**: Explain the process of creating and implementing a Custom User Model in Django, including the necessary changes to settings.py and the required model fields.

**Qp2**: Write in the format of a recipe.


**A**: Creating and Implementing a Custom User Model in Django:

Ingredients:

Django project
Python
Instructions:

Create a new Django app:

Run python manage.py startapp <app_name>, replacing <app_name> with your desired name.
Define the Custom User Model:

In the new app, create or open models.py.
Import necessary modules: AbstractBaseUser, BaseUserManager, PermissionsMixin, and models.
Define CustomUserManager class with create_user and create_superuser methods.
Define CustomUser class inheriting from AbstractBaseUser and PermissionsMixin.
Include fields like email, first_name, last_name, is_active, and is_staff.
Assign CustomUserManager() to the objects attribute.
Set USERNAME_FIELD and REQUIRED_FIELDS.
Update settings.py:

In your project's settings.py, add AUTH_USER_MODEL = '<app_name>.CustomUser', replacing <app_name> with your app's name.
Create and apply migrations:

Run python manage.py makemigrations and python manage.py migrate.
Update admin.py (optional):

Import UserAdmin, your CustomUser, and admin.
Define CustomUserAdmin class inheriting from UserAdmin.
Customize attributes such as model, list_display, list_filter, fieldsets, add_fieldsets, search_fields, and ordering.
Register your CustomUser with CustomUserAdmin using admin.site.register().
Your Custom User Model in Django is now ready for use!


**Qp**:What is DjangoX and how does it complement or extend the functionality of Django? Provide an example use case for incorporating DjangoX in a project.

**A**: DjangoX complements the functionality of Django by providing the following features:

Pre-configured user authentication, including signup, login, and password reset functionality.
Pre-configured static file handling, enabling developers to focus on building the application.
Pre-configured settings for different environments, such as development, staging, and production.
Integration of popular third-party packages, such as Django REST framework, Django Allauth, and Django Crispy Forms, to enhance the application's functionality.
Pre-configured test settings, allowing developers to quickly start writing tests for their application.
Built-in support for continuous integration and deployment, improving development workflow.
Example use case for incorporating DjangoX in a project:

Suppose you are building an e-commerce web application with Django. Instead of starting from scratch and manually configuring user authentication, static file handling, and other settings, you can use the DjangoX project template. This will save you time and effort by providing a pre-configured environment with useful packages and libraries already integrated.

With DjangoX, you can quickly begin focusing on the e-commerce-specific aspects of your application, such as product management, shopping cart functionality, and payment processing, while benefiting from the best practices and pre-configured components provided by DjangoX.

## Sources & Resources:

ChatGPT 

https://learndjango.com/tutorials/django-custom-user-model

https://github.com/wsvincent/djangox

https://docs.djangoproject.com/en/3.0/topics/auth/customizing/#auth-custom-user

https://www.youtube.com/watch?v=EudKs1HPUfE

## Things I want to know more about

DEBUG and Admin Settings 
Custom Models 


