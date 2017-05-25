# <p align="center"> Hello World app </p>

Let us build a sample hello world app using laravel.

* ### Step-1:

Create a new app using the below command, in the laravel directory

```$ laravel new app```

This will install all the dependencies required for the app to run, such that it takes some time.

Now your app is created.

Before creating developing the app, let us know some basics about routing.

The most basic Laravel routes simply accept a URI and a Closure, providing a very simple and expressive method of defining routes:
```
Route::get('foo', function () {
    return 'Hello World';
});
```
**The Default Route Files**

All Laravel routes are defined in your route files, which are located in the routes directory. These files are automatically loaded by the framework. The routes/web.php file defines routes that are for your web interface. These routes are assigned the web middleware group, which provides features like session state and CSRF protection. The routes in routes/api.php are stateless and are assigned the api middleware group.

For most applications, you will begin by defining routes in your routes/web.php file.

Note: In older version, laravel routes are defined directly in routes.php.

* ### Step-2:

Now open web.php which is located in he routes directory.

This may look like this
```
<?php

Route::get('/', function () {
    return view('welcome');
});
```
* ### Step-3:

Now open welcome.blade.php in the view directory, and change the code in the below styling
```
<!DOCTYPE html>
<html>
<head>
    <title></title>
</head>
<body>
<h1>Hello world</h1>
</body>
</html>
```
Note: Above styling is just an example, you can change in your own styling.

* ### Step-4:

Run the below command,

```$ php artisan serve```

This command will start a development server at http://localhost:8000: 

Your output will look like this

![Hello world](hello.png)

* ### Step-5:

If you want to create an other page for example 'about' page

Add the below code, after the root function
```
Route::get('about', function () {
    return view('about');
});
```
* ### Step-6:

Now create a new file in the views directory, and change the name of the file to about.blade.php then add the styling.

for example:
```
<!DOCTYPE html>
<html>
<head>
    <title></title>
</head>
<body>
<h1>About us</h1>
</body>
</html>
```
Now save the file. Make sure the file is in the views directory.

* ### Step-7:

Now start the server, by using the below command.

```$ php artisan serve```

This command will start a development server at http://localhost:8000: 

Now if you want view the about page, then change the url to http://localhost:8000/about

Your output will look like this

![AboutUs](about.png)















