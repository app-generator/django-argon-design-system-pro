# [Django Argon System PRO](https://appseed.us/product/argon-design-system-pro/django/)

Seed project generated by AppSeed in **Flask** Framework on top of **Argon Design System PRO** with database, authentication, helpers and Docker support. Argon Design System PRO is built with over 1100 individual elements, 43 sections and 17 example pages giving you the freedom of choosing and combining. 

- 👉 [Django Argon System PRO](https://appseed.us/product/argon-design-system-pro/django/) - product page
- 👉 [Django Argon System PRO](https://django-argon-design-system-pro.appseed-srv1.com/) - LIVE App
- 👉 [Complete documentation](https://docs.appseed.us/boilerplate-code/django) - `Learn how to use and update the product`

<br />

> Features

- `Up-to-date dependencies`
- Database: `sqlite`
- UI-Ready app, Django Native ORM
- **Authentication**
  - `Session-Based authentication`

<br />

![Argon Design PRO - Seed project crafted by AppSeed.](https://user-images.githubusercontent.com/51070104/187922792-7f7c8bb9-25a5-4129-a0fe-6bbfba82501d.png)

<br />

## ✨ Start the app in Docker

> **Step 1** - Download the [code](https://appseed.us/product/argon-design-system-pro/django/) and unzip the sources (requires a `purchase`). 

```bash
$ # Get the code
$ unzip django-argon-design-system-pro.zip
$ cd django-argon-design-system-pro
```

<br />

> **Step 2** - Start the APP in `Docker`

```bash
$ docker-compose up --build 
```

Visit `http://localhost:5085` in your browser. The app should be up & running.

<br />

## ✨ How to use it

> Download the [code](https://appseed.us/product/argon-design-system-pro/django/) and unzip the sources (requires a `purchase`). 

```bash
$ # Get the code
$ unzip django-argon-design-system-pro.zip
$ cd django-argon-design-system-pro
```

<br />

### 👉 Set Up for `Unix`, `MacOS` 

> Install modules via `VENV`  

```bash
$ virtualenv env
$ source env/bin/activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> Create Superuser

```bash
$ python manage.py createsuperuser
```

<br />

> Start the app

```bash
$ python manage.py runserver
// OR with https
$ python manage.py runsslserver 
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

### 👉 Set Up for `Windows` 

> Install modules via `VENV` (windows) 

```
$ virtualenv env
$ .\env\Scripts\activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> Create Superuser

```bash
$ python manage.py createsuperuser
```

<br />

> Start the app

```bash
$ python manage.py runserver
// OR with https
$ python manage.py runsslserver 
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

## ✨ Create Users

By default, the app redirects guest users to authenticate. In order to access the private pages, follow this set up: 

- Start the app via `flask run`
- Access the `registration` page and create a new user:
  - `http://127.0.0.1:8000/register/`
- Access the `sign in` page and authenticate
  - `http://127.0.0.1:8000/login/`

<br />

## Recompile SCSS

> Navigate to `apps/static/assets` and execute the gulp command default task in the directory. 

Compilation tests were made with:

- **Node** `v16.15.0`
- **Gulp** `v4.0.2`, CLI version `4.0.2`

```bash
$ cd apps/static/assets
$ yarn                   # install modules
$ gulp                   # recompile SCSS
```

<br />

## ✨ Code-base structure

The project is coded using a simple and intuitive structure presented below:

```bash
< PROJECT ROOT >
   |
   |-- core/                               # Implements app configuration
   |    |-- settings.py                    # Defines Global Settings
   |    |-- wsgi.py                        # Start the app in production
   |    |-- urls.py                        # Define URLs served by all apps/nodes
   |
   |-- apps/
   |    |
   |    |-- home/                          # A simple app that serve HTML files
   |    |    |-- views.py                  # Serve HTML pages for authenticated users
   |    |    |-- urls.py                   # Define some super simple routes  
   |    |
   |    |-- authentication/                # Handles auth routes (login and register)
   |    |    |-- urls.py                   # Define authentication routes  
   |    |    |-- views.py                  # Handles login and registration  
   |    |    |-- forms.py                  # Define auth forms (login and register) 
   |    |
   |    |-- static/
   |    |    |-- <css, JS, images>         # CSS files, Javascripts files
   |    |
   |    |-- templates/                     # Templates used to render pages
   |         |-- includes/                 # HTML chunks and components
   |         |    |-- navigation.html      # Top menu component
   |         |    |-- sidebar.html         # Sidebar component
   |         |    |-- footer.html          # App Footer
   |         |    |-- scripts.html         # Scripts common to all pages
   |         |
   |         |-- layouts/                   # Master pages
   |         |    |-- base.html             # Used by common pages
   |         |
   |         |-- accounts/                  # Authentication pages
   |         |    |-- login.html            # Login page
   |         |    |-- register.html         # Register page
   |         |
   |         |-- home/                      # UI Kit Pages
   |              |-- index.html            # Index page
   |              |-- page-404.html         # 404 page
   |              |-- *.html                # All other pages
   |
   |-- requirements.txt                     # Development modules - SQLite storage
   |
   |-- .env                                 # Inject Configuration via Environment
   |-- manage.py                            # Start the app - Django default start script
   |
   |-- ************************************************************************
```

<br />

---
[Django Argon System PRO](https://appseed.us/product/argon-design-system-pro/django/) - Seed project generated by **[AppSeed Generator](https://appseed.us/generator/)**.
