# Ex02 Django ORM Web Application
## Date: 5-5-2025

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![Screenshot 2024-12-09 114339](https://github.com/user-attachments/assets/b3c6db24-b57c-4098-abe4-6036f35077f1)


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
from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)

from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
     serialno=models.IntegerField(primary_key="serialno");
     bookname=models.CharField(max_length=20);
     publisher=models.CharField(max_length=20);
     Dop=models.DateField();
     totalpg=models.IntegerField();
class Book_DBAdmin(admin.ModelAdmin):
     list_display=("serialno","bookname","publisher","Dop","totalpg");

```


## OUTPUT
![Screenshot 2024-03-05 110658](https://github.com/user-attachments/assets/e0e2a208-8843-4ae3-93fe-704b2f34283b)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
