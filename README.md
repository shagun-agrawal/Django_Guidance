# Django_Guidance
# why django is used
(django is a frame work of python programming which is used to make web appl
ication it makes easy to create website )


# if you wona install django in vertual enviroment 
step(1): go to in your virtual enviroment
step(2): write cmd "pip install django==(django version name)"
step(3): By cmd "django-admin --version" you can chack it is installed or not

# for create first project
step(1):go to in your virtual enviroment
step(2):write cmd "django-admin startproject (project name like first_project)" 
step(3):go inside your first_project by cmd in this project you will get a manage.py file by this file
        you can run your server with command "python manage.py runserver" you will get a link and paste this 
        link into the chrome.
step(4):open your project in any IDE(Intigrated Development Enviroment) like VScode
step(5):To create your app(it is a combination of web pages)
step(6):you have to write cmd "python manage.py startapp (AppName like first_app)"
step(7):there will be multile files in your app but there will not be urls
        file so first you have to make ulrs file in your app
step(8):after making urls file you have to import path in urls file
        "from django.urls import path" 
step(9):if you wona went to another page from one page so you have to 
        import views(it will provide a facilty to go one page to another page)
        "from . import views"
step(10):you have to make a list of ulrpatterns in urls file
         "urlpatterns=[path('',views.home,name="home")]"
         (views.home=it will call home function in your app's views file)
         (name=it is the name of the page)
step(11):you have to make and home function in to the views file 
         open app's views file and make home function
        "def home(request):
               return HttpResponse("Hellow This Is Shagun")
        "
        this function will return HttpResponse() function and whatever you will
        pass the string will show into your home page
  Note: you have to import a package in your views file "from django.http import HttpResponse"

step(12):your app will be created 
step(13):you have to link your app with your project
           (1):open your project's urls file
           (2):make a path in urlpatterns
           (3):"path('',include('first_app.urls')),"
           (4):you have to import include "from django.urls import include"
step(14): now you can run your server with terminal "python manage.py runserver"
          copy the link and paste in your chrome
