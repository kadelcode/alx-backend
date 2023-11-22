# i18n (Internationalization)
- The process of designing and developing software so that it can be adapted to different languages and cultures without engineering changes.

## Resources
Read or watch:

- [Flask-Babel](https://flask-babel.tkte.ch/)
- [Flask i18n tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-xiii-i18n-and-l10n)
- [pytz](https://sourceforge.net/directory/software-development/windows/)

## Learning Objectives
- Learn how to parametrize Flask templates to display different languages
- Learn how to infer the correct locale based on URL parameters, user settings or request headers
- Learn how to localize timestamps

## Requirements
- All your files will be interpreted/compiled on Ubuntu 18.04 LTS using python3 (version 3.7)
- All your files should end with a new line
- A ```README.md``` file, at the root of the folder of the project, is mandatory
- Your code should use the pycodestyle style (version 2.5)
- The first line of all your files should be exactly ```#!/usr/bin/env python3```
- All your ```*.py``` files should be executable
- All your modules should have a documentation (```python3 -c 'print(__import__("my_module").__doc__)'```)
- All your classes should have a documentation (```python3 -c 'print(__import__("my_module").MyClass.__doc__)'```)
- All your functions and methods should have a documentation (```python3 -c 'print(__import__("my_module").my_function.__doc__)'``` and ```python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'```)
- A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class or method (the length of it will be verified)
- All your functions and coroutines must be type-annotated.

## Tasks
### 0. Basic Flask app
First you will setup a basic Flask app in ```0-app.py```. Create a single / route and an ```index.html``` template that simply outputs “Welcome to Holberton” as page title (```<title>```) and “Hello world” as header (```<h1>```).

### 1. Basic Babel setup
Install the Babel Flask extension:
```
$ pip3 install flask_babel==2.0.0
```
Then instantiate the ```Babel``` object in your app. Store it in a module-level variable named ```babel```.

In order to configure available languages in our app, you will create a ```Config``` class that has a ```LANGUAGES``` class attribute equal to ```["en", "fr"]```.

Use ```Config``` to set Babel’s default locale (```"en"```) and timezone (```"UTC"```).

Use that class as config for your Flask app.
