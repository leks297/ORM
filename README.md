# Ex02 Django ORM Web Application
# Date:26-11-2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM
from django.contrib import admin
from .models import owner,ownerAdmin
admin.site.register(owner,ownerAdmin)

from django.db import models
from django.contrib import admin
class owner(models.Model):
    car_no=models.IntegerField()
    colour=models.CharField(max_length=10)
    product_no=models.IntegerField()
    brand=models.CharField(max_length=10)
class ownerAdmin(admin.ModelAdmin):
    list_display=["car_no","colour","product_no","brand"]   


# OUTPUT
Include the screenshot of your admin page.
<img width="1266" height="512" alt="ORM OUTPUT" src="https://github.com/user-attachments/assets/b61d4306-e44d-4cfe-9a39-e82f734b07d6" />

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
