# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
model.py
from django.db import models
from django.contrib import admin
class Car(models.Model):
    brand_name=models.CharField(max_length=20)
    car_name=models.CharField(max_length=10)
    enginenum=models.IntegerField()
    release_date=models.DateField()

class CarAdmin(admin.ModelAdmin):
    list_display=('brand_name', 'car_name', 'enginenum', 'release_date')
admin.py
from django.contrib import admin
from.models import Car,CarAdmin
admin.site.register(Car,CarAdmin)
```



## OUTPUT


![alt text](<Screenshot 2025-11-21 112737.png>) 
![alt text](<Screenshot 2025-11-21 131001.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
