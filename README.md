# Ex02 Django ORM Web Application
# Date:25-11-2025
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
```
admin.py 

from django.contrib import admin
from .models import car,carAdmin
admin.site.register(car,carAdmin)


models.py

from django.db import models
from django.contrib import admin
class car(models.Model):
    car_name=models.CharField(max_length=20)
    car_model=models.IntegerField()
    car_colour=models.CharField(max_length=20)
    year_of_released=models.DateField()
    on_road_price=models.CharField()
class carAdmin(admin.ModelAdmin):
    list_display=["car_name","car_model","car_colour","year_of_released","on_road_price"]

```


# OUTPUT
![alt text](<Screenshot 2025-11-25 201413.png>)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
