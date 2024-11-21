## INSTALLED LIBRARIES

## 1. asgiref
### What it is: A library that provides utilities for building ASGI (Asynchronous Server Gateway Interface) applications, which is the newer standard for Python web applications.
### Why it’s used:
Required by Django for asynchronous support(handling multiple tasks at the same time) .
Helps handle asynchronous tasks like WebSockets and HTTP/2.
#### Use case: Installed automatically with Django 3.1+ to enable async capabilities.
## 2. Django
### What it is: A popular Python web framework for building web applications quickly and securely.
### Why it’s used:
Comes with tools for handling databases, user authentication, admin interfaces, and more.
Encourages rapid development with reusable components.
#### Use case: Create scalable and secure web applications.
## 3. django-cors-headers
### What it is: A Django app for managing Cross-Origin Resource Sharing (CORS) headers.
Cross-Origin Resource Sharing (CORS) is a security feature that helps manage how web pages hosted on one domain can interact with resources (like APIs) hosted on a different domain.
### Why it’s used:
Ensures frontend apps (e.g., React, Angular) hosted on **different domains** can communicate with your Django backend.
Helps avoid CORS errors when using APIs.
### Use case:
Add CORS headers to Django responses to allow cross-origin requests.
## 4. djangorestframework (DRF)
### What it is: A powerful toolkit for building Web APIs in Django.
### Why it’s used:
Makes it easy to create RESTful APIs for your Django app.
Includes serializers, authentication, and permission systems.
#### Use case: Build APIs to connect Django backends with frontend or mobile apps.
## 5. djangorestframework-simplejwt
### What it is: A library for JSON Web Token (JWT) authentication in Django REST Framework.
### Why it’s used:
Simplifies implementing token-based authentication.
Provides secure user authentication with JWTs.
#### Use case: Protect API endpoints by requiring users to provide valid JWTs.
## 6. PyJWT
### What it is: A Python library for encoding and decoding JSON Web Tokens (JWTs).
### Why it’s used:
Works with JWT-based authentication systems.
Supports signing and verifying JWTs.
#### Use case: Generate and verify JWTs when implementing authentication systems.
## 7. pytz
### What it is: A library for handling time zones in Python.
### Why it’s used:
Provides access to the IANA time zone database.
Helps ensure time zone-aware datetime handling.
#### Use case: Convert datetime objects between time zones in your application.
## 8. sqlparse
### What it is: A library for parsing, formatting, and analyzing SQL queries.
### Why it’s used:
Formats raw SQL queries into readable formats.
Used internally by Django to handle SQL query strings.
### Use case: Automatically included in Django for database query handling.
## 9. psycopg2-binary
### What it is: A PostgreSQL adapter for Python.
### Why it’s used:
Allows Django (or any Python app) to interact with a PostgreSQL database.
Provides a simple API for executing SQL queries.
#### Use case: Connect your Django app to a PostgreSQL database.
## 10. python-dotenv
### What it is: A library to read environment variables from a .env file.
### Why it’s used:
Helps manage sensitive information like API keys, database credentials, etc., without hardcoding them.
Simplifies configuration for local development.
#### Use case: Load settings (e.g., DATABASE_URL) from a .env file into your app’s environment.


# How They Work Together in a Django Project:
**Django:** The core web framework.

**DRF and DRF-SimpleJWT:** For building APIs and adding JWT-based authentication.

**PyJWT:** Underlying library used by SimpleJWT to handle tokens.

**psycopg2-binary:** Connects Django to a PostgreSQL database.

**python-dotenv:** Manages environment variables securely.

**pytz:** Ensures time zone handling in Django’s datetime operations.

**django-cors-headers:** Allows frontend apps to call Django APIs without CORS errors.

**sqlparse:** Helps format SQL queries, used internally by Django.
