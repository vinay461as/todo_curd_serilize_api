# todo_curd_serilize_api
This is a TODO API, it consist of create, update, read and delete operations

# Install Required Packages
The project was built and tested with Django 3.x version.The Django project need some Python package to install
```
pip install Django
pip install djangorestframework
```

# Running the Application
Before running the application we need to create the needed DB tables:
```
python manage.py makemigrations
python manage.py migrate
 ```
Now run the server
```
python manage.py runserver
```
To access the applications, go to the URL http://localhost:8000/

This will show an overview page that consist of a list of url related to curd_api

```
HTTP 200 OK
Allow: OPTIONS, GET
Content-Type: application/json
Vary: Accept

{
    "List": "/todo-list/",
    "Detail": "/todo-detail/<str:pk>/",
    "Create": "/todo-create/",
    "Update": "/todo-update/<str:pk>/",
    "Delete": "/todo-delete/<str:pk>/"
}
```
