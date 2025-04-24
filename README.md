# Ex02 Django ORM Web Application
## Date: 
## Name: Elaiyavan 
## Roll No:2100

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).


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
admin.py 

from django.contrib import admin
from .models import Movie

admin.site.register(Movie)

```
```
model.py

from django.db import models

class Movie(models.Model):
    title = models.CharField(max_length=200)
    director = models.CharField(max_length=100)
    release_year = models.PositiveIntegerField()
    genre = models.CharField(max_length=100)

    def __str__(self):
        return f"{self.title} ({self.release_year})"

```


## OUTPUT

![alt text](<Screenshot 2025-04-24 091352.png>)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
