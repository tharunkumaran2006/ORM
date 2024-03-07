# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![Screenshot 2024-03-07 133620](https://github.com/Narasimhan05/ORM/assets/132819871/f6cf46de-e5e5-4848-8f3f-fab81fb15673)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM

```
models.py

from django.db import models
from django.contrib import admin
class Library(models.Model):
   book=models.CharField(max_length=30);
   bookid=models.IntegerField(primary_key=True);
   author=models.CharField(max_length=30);
   dept=models.CharField(max_length=30);
   publisher=models.CharField(max_length=30);
class LibraryAdmin(admin.ModelAdmin):
   list_display=('book','bookid','author','dept','publisher');


   admin.py

   from django.contrib import admin
from .models import Library,LibraryAdmin
admin.site.register(Library,LibraryAdmin)                                                                                   
```

## OUTPUT

![image](https://github.com/Narasimhan05/ORM/assets/132819871/1acd1a6b-559a-4095-8946-8727a9e4548e)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
