# 401 Advanced Python: Class 32 Reading Notes

## Summary: This class reading is about: Permissions & Postgresql

- Django Rest Framework (DRF) permissions are essential for controlling access to API resources. Key components include permission classes and authentication mechanisms. The purpose is to secure the API by allowing or denying access based on user privileges, ensuring only authorized users can interact with specific resources.

- The SELECT statement in SQL is used to query and retrieve data from one or more tables in a database. To retrieve all columns from a table called 'employees', you would use the following query: SELECT * FROM employees;

Query: SELECT * FROM employees;

Result:
+----+-----------+-----------+--------+------------+
| id | first_name| last_name | salary | hire_date  |
+----+-----------+-----------+--------+------------+
|  1 | John      | Doe       | 50000  | 2020-01-01 |
|  2 | Jane      | Smith     | 60000  | 2019-06-15 |
|  3 | Alice     | Johnson   | 45000  | 2021-02-28 |
+----+-----------+-----------+--------+------------+

- DRF Generic Views simplify common tasks in building RESTful APIs by providing pre-built, reusable view classes. They handle standard CRUD operations, reducing code redundancy and improving maintainability. Examples include ListCreateAPIView, RetrieveUpdateDestroyAPIView, and ListAPIView.


## Re/Sources: 

ChatGPT 

https://codefellows.github.io/common_curriculum/prework/SQL

https://www.cdrf.co/

https://www.django-rest-framework.org/api-guide/generic-views/

https://www.django-rest-framework.org/api-guide/permissions/
