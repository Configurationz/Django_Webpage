Creating a sample django web application work on windows
---------------------------------------------------------

*  [Refer Here](https://chocolatey.org/install#individual) to install Chocolatey on Windows 10/11

* To install Python 3.11, run the following command from PowerShell _(Run as Administrator)_:
```
choco install python311
```
* All supported versions of python3 include pip, so just make sure it’s updated:
```
python -m pip install -U pip
```

* So, coming back to our project i.e., [django framework](https://docs.djangoproject.com/en/4.2/intro/tutorial01/)

1. Create a folder anywhere in your local m/c
```
mkdir django-starter
cd .\django-starter\
```

2. Run the following command inside django-starter\
```
python -m venv .venv
```

3. Next, Execute the following
```
.\.venv\Scripts\activate
```

4. Install Django
```
pip install django
```

5. Now, let's create the project
```
django-admin startproject mysite
```

6. A new directory is created which is _mysite_
```
cd .\mysite\
```

7. Let’s verify if the Django project works
```
python manage.py runserver
```

* You’ll get the following output on the command line:

```php
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).

You have 18 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
Run 'python manage.py migrate' to apply them.
September 23, 2023 - 22:11:35
Django version 4.2.5, using settings 'mysite.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CTRL-BREAK.

[23/Sep/2023 22:12:04] "GET / HTTP/1.1" 200 10664
Not Found: /favicon.ico
[23/Sep/2023 22:12:04] "GET /favicon.ico HTTP/1.1" 404 2110
```

8. Finally, access the django web application
```
http://127.0.0.1:8000/
```
## Reference

> _**[Django Project](https://docs.djangoproject.com/en/4.2/intro/tutorial01/)**_