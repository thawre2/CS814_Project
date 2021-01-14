# CS814_Project
## Table of Contents
* [Applications needed to run program](#applications-needed-to-run-program)
* [How to install and run code](#how-to-install-and-run-code)
* [Specification about application](#specification-about-application)
* [Settings of Code](#settings-of-code)

## Applications needed to run program
* IDE: Visual Studio Code
* Language: HTML, CSS, Python
* Server: Django
* Database: SQLite (which is inbuilt with Django)
## How to install and run code
* Install Python3 (any version will do)
* Open Terminal and Execute Following Commands:

Python3 -m pip install -r requirements.txt

* Make pull of the code using

git pull url

* Move to the project folder in terminal, then run following commands: 

python3 manage.py makemigrations

python3 manage.py migrate

python3 manage.py runserver

* Enter the following URL in Browser:

http://127.0.0.1:8000/

## Specification about application
### Admin
* Create Admin account and Login.
* Can Add, View, Book
* Can Issue Book (added by Admin) to registered student.
* Can view Issued book with issued date and expiry date.
* Can view Fine (10 rupees for each day after expiry date).
* Can view Students that are registered into system.

### Student
* Create account and Login.
* Can view their issued book only with expiry date and fine (if there any, otherwise 0)

## Settings of code
pip3 install django-role-permissions

Add rolepermissions in out INSTALLED_APPS

INSTALLED_APPS = {
      
      'rolepermissions',
     
}
