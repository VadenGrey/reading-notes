# Class 32

**DRF Permissions**

Together with authentication and throttling, permissions determine whether a request should be granted or denied access.

Permission checks are always run at the very start of the view, before any other code is allowed to proceed. Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.

Before running the main body of the view each permission in the list is checked. If any permission check fails, an exceptions.PermissionDenied or exceptions.NotAuthenticated exception will be raised, and the main body of the view will not run.

**Review SQL Prework**

SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

references

[DRF Permissions](https://www.django-rest-framework.org/api-guide/permissions/)

[Review SQL Prework](https://codefellows.github.io/common_curriculum/prework/SQL)

<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)