# why django is used<br>
(django is a frame work of python programming which is used to make web appl<br>
<br>
ication it makes easy to create website )
<br>

# If you wona install django in vertual enviroment 
<br>
<h3>step(1):</h3> go to in your virtual enviroment<br>
<br> <h3>step(2):</h3> write cmd "pip install django==(django version name)"
<br><h3>step(3):</h3> By cmd "django-admin --version" you can chack it is installed or not

<br># for create first project
<br><h3>step(1):</h3>go to in your virtual enviroment
<br><h3>step(2):</h3>write cmd "django-admin startproject (project name like first_project)" 
<br><h3>step(3):</h3>go inside your first_project by cmd in this project you will get a manage.py file by this file
    <br>    you can run your server with command "python manage.py runserver" you will get a link and paste this 
        <br>link into the chrome.
<br><h3>step(4):</h3>open your project in any IDE(Intigrated Development Enviroment) like VScode
<br><h3>step(5):</h3>To create your app(it is a combination of web pages)
<br><h3>step(6):</h3>you have to write cmd "python manage.py startapp (AppName like first_app)"
<br><h3>step(7):</h3>there will be multile files in your app but there will not be urls
    <br>    file so first you have to make ulrs file in your app
<br><h3>step(8):</h3>after making urls file you have to import path in urls file
   <br>     "from django.urls import path" 
<br><h3>step(9):</h3>if you wona went to another page from one page so you have to 
    <br>    import views(it will provide a facilty to go one page to another page)
       <br> "from . import views"
<br><h3>step(10):</h3>you have to make a list of ulrpatterns in urls file
    <br>     "urlpatterns=[path('',views.home,name="home")]"
        <br> (views.home=it will call home function in your app's views file)
         <br>(name=it is the name of the page)
<br><h3>step(11):</h3>you have to make and home function in to the views file 
    <br>     open app's views file and make home function
        <br>"def home(request):
            <br>   return HttpResponse("Hellow This Is Shagun")
        <br>"
      <br>  this function will return HttpResponse() function and whatever you will
        <br>pass the string will show into your home page
 <br> Note: you have to import a package in your views file "from django.http import HttpResponse"

<br><h3>step(12):</h3>your app will be created 
<br><h3>step(13):</h3>you have to link your app with your project
    <br>       (1):open your project's urls file
     <br>      (2):make a path in urlpatterns
         <br>  (3):"path('',include('first_app.urls')),"
           <br>(4):you have to import include "from django.urls import include"
<br><h3>step(14):</h3> now you can run your server with terminal "python manage.py runserver"
    <br>      copy the link and paste in your chrome
