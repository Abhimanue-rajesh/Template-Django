<h1 align="center">Django Template</h1>

[![Django CI](https://github.com/Abhimanue-rajesh/Template-Django/actions/workflows/django.yml/badge.svg)](https://github.com/Abhimanue-rajesh/Template-Django/actions/workflows/django.yml)

![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)
![JQuery](https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white)
![NGINX](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Debian](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)
![Warp](https://img.shields.io/badge/warp-01A4FF?style=for-the-badge&logo=warp&logoColor=white)


## Overview:
This is a Template

## Setting up environment

### Prerequisites

Before starting, ensure you have the following installed on your system:

- Python (preferably version 3.11.7 or above)
- Pip (Python package installer)
- Virtual environment (optional but recommended for creating isolated Python environments)

**Create a Virtual Environment**

> [!CAUTION]
> Not creating a virtual environment can lead to project instability.

Creating a virtual environment helps isolate your project dependencies from other Python projects on your system. To create a virtual environment, run the following commands in your terminal:

1. Create a virtual environment named 'venv'
    ```bash
    python -m venv venv
    ```
2. Activating the environment

- For windows
    ```bash
    venv\Scripts\activate
    ```
- For macOS and Linux
    ```bash
    source venv/bin/activate
    ```

**Installing all the required libraries**

Now that you have a virtual environment set up, you can install Django and other libraries required within the project:

```bash
pip install -r requirements.txt
```

**Running the project in your local system**

Before running ensure that the :
1. Virtual Environment is activated

Run Migrations

```bash
python manage.py migrate
```

Then a super user has to be created
```bash
python manage.py createsuperuser
```

Then run the program in the development server
```bash
python manage.py runserver
```

**Creating and filling the database table with fake data**

1. To Populate user fake data
```bash
python manage.py populate_user_data
```

2. To populate project fake data
```bash
python manage.py populate_project_data
```

**Development Requirements**
1. Needed Extensions
    1.1. Flake8
    1.2. mypy

2. Running pre commit before a commit

Only Clean when needed

```bash
pre-commit install
```

```bash
pre-commit run --all-files
```

```bash
pre-commit clean
```

## Run Test

```bash
python manage.py test
```
