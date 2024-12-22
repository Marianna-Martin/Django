django-admin startproject nameofproject

cd (directory of the project)

django-admin startapp api

project->project->settings.py->INSTALLED_APPS #addline 'api.apps.ApiConfig','rest_framework'


In a Django project, each app (like api) can have a configuration class. ApiConfig is where you define settings specific to that app, such as its name or default behaviors.

#Go To views.py
1. What Does views.py Do?
It connects URLs to the logic that handles them.
Processes HTTP requests (GET, POST, etc.) sent by the user.
Returns HTTP responses, such as web pages, JSON data, or error messages.
Acts as the bridge between your models (database) and templates (HTML).

Why is views.py Important?
It’s where you define how your app behaves.

It ensures a clean separation of logic (views) from presentation (templates).

Essential for creating dynamic and interactive web applications!

create a file namaed urls.py under api


## 2.  MODELS.PY -defines databases











