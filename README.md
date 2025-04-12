# Ex02 Django ORM Web Application
## Date: 05/04/2025
## NAME: Elaiyavan.k

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

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
### admin.py
```
from django.contrib import admin
from .models import Loan,LoanAdmin
admin.site.register(Loan,LoanAdmin)
```
### models.py
```
from django.db import models
from django.contrib import admin
class Loan(models.Model):
   Customerid=models.CharField(max_length=20, primary_key=True)
   Customername=models.CharField(max_length=100)
   Mobile=models.IntegerField( )
   Age=models.IntegerField( )
   Email=models.EmailField( )
   DOB=models.DateField( )
   Loan_amount=models.IntegerField( )
class LoanAdmin(admin.ModelAdmin):
    list_display=('Customerid','Customername','Mobile','Age','Email','DOB','Loan_amount')

```
## OUTPUT
![WhatsApp Image 2024-12-07 at 10 48 41 PM](https://github.com/user-attachments/assets/65e9e71a-6c8e-4da4-959e-715097a2981a)


![Screenshot 2025-04-12 112316](https://github.com/user-attachments/assets/1ef53e40-7070-4c39-8e48-ce07daa781ee)


![Screenshot 2025-04-12 112325](https://github.com/user-attachments/assets/c8b16186-c837-4db7-ad94-9f14c2d543df)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
