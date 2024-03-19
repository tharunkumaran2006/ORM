# Ex02 Django ORM Web Application
## Date: 27.02.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## ENTITY RELATINSHIP DIAGRAM
![ER Diagram](https://github.com/tharunkumaran2006/ORM/assets/151625188/bf07db08-08c2-48e1-91df-89858b983483)



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
class Books(models.Model):
	bookno         = models.IntegerField(primary_key=True);
	bookname       = models.CharField(max_length=20);
	author         = models.CharField(max_length=20);
	pages          = models.IntegerField();
	published_date = models.DateField();
	bookprice      = models.IntegerField();
class BooksAdmin(admin.ModelAdmin):
	list_display=("bookno","bookname","author","pages","published_date","bookprice");

admin.py
	
from django.contrib import admin
from.models import Books,BooksAdmin
admin.site.register(Books,BooksAdmin)
```

## OUTPUT
![Screenshot 2024-03-15 191241](https://github.com/tharunkumaran2006/ORM/assets/151625188/e3d5a5c9-db34-4962-8788-aef2d48fcb2f)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
