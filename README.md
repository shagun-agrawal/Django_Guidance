# why django is used<br>
(django is a frame work of python programming which is used to make web appl<br>
<br>
ication it makes easy to create website )
<br>

# If you wona install django in vertual enviroment 
<br>
<h1>step(1):</h1> go to in your virtual enviroment<br>
<br> <h1>step(2):</h1> write cmd "pip install django==(django version name)"
<br><h1>step(3):</h1> By cmd "django-admin --version" you can chack it is installed or not

<br># for create first project
<br><h1>step(1):</h1>go to in your virtual enviroment
<br><h1>step(2):</h1>write cmd "django-admin startproject (project name like first_project)" 
<br><h1>step(3):</h1>go inside your first_project by cmd in this project you will get a manage.py file by this file
    <br>    you can run your server with command "python manage.py runserver" you will get a link and paste this 
        <br>link into the chrome.
<br><h1>step(4):</h1>open your project in any IDE(Intigrated Development Enviroment) like VScode
<br><h1>step(5):</h1>To create your app(it is a combination of web pages)
<br><h1>step(6):</h1>you have to write cmd "python manage.py startapp (AppName like first_app)"
<br><h1>step(7):</h1>there will be multile files in your app but there will not be urls
    <br>    file so first you have to make ulrs file in your app
<br><h1>step(8):</h1>after making urls file you have to import path in urls file
   <br>     "from django.urls import path" 
<br><h1>step(9):</h1>if you wona went to another page from one page so you have to 
    <br>    import views(it will provide a facilty to go one page to another page)
       <br> "from . import views"
<br><h1>step(10):</h1>you have to make a list of ulrpatterns in urls file
    <br>     "urlpatterns=[path('',views.home,name="home")]"
        <br> (views.home=it will call home function in your app's views file)
         <br>(name=it is the name of the page)
<br><h1>step(11):</h1>you have to make and home function in to the views file 
    <br>     open app's views file and make home function
        <br>"def home(request):
            <br>   return HttpResponse("Hellow This Is Shagun")
        <br>"
      <br>  this function will return HttpResponse() function and whatever you will
        <br>pass the string will show into your home page
 <br> Note: you have to import a package in your views file "from django.http import HttpResponse"

<br><h1>step(12):</h1>your app will be created 
<br><h1>step(13):</h1>you have to link your app with your project
    <br>       (1):open your project's urls file
     <br>      (2):make a path in urlpatterns
         <br>  (3):"path('',include('first_app.urls')),"
           <br>(4):you have to import include "from django.urls import include"
<br><h1>step(14):</h1> now you can run your server with terminal "python manage.py runserver"
    <br>      copy the link and paste in your chrome
