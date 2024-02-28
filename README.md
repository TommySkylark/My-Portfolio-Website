# Data Analyst/Developer Portfolio Website

This is a data analyst/developer portfolio website built using **Django 4**, **HTML 5**, **CSS 3**, **Bootstrap 5**, and **Sass**.

![Alt text](static/images/portfolio_website.png?raw=true "Portfolio Website")




## Table of Contents 
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the application](#run-the-application)
- [Adding data to the application](#add-data-to-the-application)
- [Customizing the application](#customize-the-application)


### Prerequisites

Install the following prerequisites:

1. [Python 3.8-3.12](https://www.python.org/downloads/)
<br> This project uses **Django v4.2.4**. For Django to work, you must install a correct version of Python on your machine. More information [here](https://django.readthedocs.io/en/stable/faq/install.html).
2. [Node.js](https://nodejs.org/en/)
3. [Visual Studio Code](https://code.visualstudio.com/download) with the **Live Sass Compiler** extension.<br>

[Live Sass Compiler] extension in VSC allows us to compile Sass files to CSS files in real-time. It will watch a Sass file for changes, and then it will automatically compile that Sass file into a CSS file whenever a change is made and saved.


### Installation

#### 1. Create a virtual environment

From the **root** directory, run:

```bash
python -m venv venv
```

#### 2. Activate the virtual environment

From the **root** directory, run:

On macOS:

```bash
source venv/bin/activate
```

On Windows:

```bash
venv\scripts\activate
```

#### 3. Install required dependencies

From the **root** directory, run:

```bash
pip install -r requirements.txt
```

From the **root** directory, run:

```bash
cd static
```
```bash
npm install
```

#### 4. Run migrations

From the **root** directory, run:

```bash
python manage.py makemigrations
```
```bash
python manage.py migrate
```

#### 5. Create an admin user to access the Django Admin interface

From the **root** directory, run:

```bash
python manage.py createsuperuser
```

When prompted, enter a username, email, and password.

### Run the application

From the **root** directory, run:

```bash
python manage.py runserver
```

### View the application

Go to http://127.0.0.1:8000/ to view the application.

### Add data to the application

Add data through Django Admin.

Go to http://127.0.0.1:8000/admin to access the Django Admin interface and sign in using the admin credentials.

### Customize the application

This section describes how to customize the application. 

#### Changing Section Titles and Subtitles 

#### 1. About

To modify the title and subtitle of the **About** section, make changes in the ```templates/index.html``` file.

#### 2. Projects

To modify the title and subtitle of the **Projects** section, make changes in the ```templates/index.html``` file.

#### 3. Admin

To modify the admin tab and change the way you upload files, make changes in ```models.py``` and ```admin.py```

#### Changing Colors

To modify the colors in the application, make changes in the ```static/sass/styles.scss``` file and compile the file using the **Live Sass Compiler**, which is a Visual Studio Code Extension. Remember to set the **savePath** option in the **settings.json** file (**liveSassCompile.settings.formats** section) to **static/css** so that the generated CSS file is stored in the static/css directory. 

Note: if you your liveSassCompile doesn't work.
Use those commands:
1)To install sass

```bash
sudo npm install -g sass
```

2)Running sass

```bash
sass static/sass/styles.scss 
```

```bash
static/css/styles.css 
```

#### Changing Logo

To modify the logo in the application, make changes in the ```templates/index.html``` file.


# Portfolio-Website# Portfolio-Website
