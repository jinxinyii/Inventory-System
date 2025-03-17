# Inventory System

This is a project to practice using Python Django with a PostgreSQL database and Tailwind CSS for the front end.

## Project Structure

```
inventory_system/
    manage.py
    accounts/
        __init__.py
        admin.py
        apps.py
        forms.py
        models.py
        tests.py
        views.py
        migrations/
            __init__.py
            0001_initial.py
        templates/
            dashboard.html
            index.html
            login.html
            register.html
    inventory_system/
        __init__.py
        asgi.py
        settings.py
        urls.py
        wsgi.py
```

## Setup Instructions

1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd inventory_system
    ```

2. Create a virtual environment and activate it:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the dependencies:
    ```sh
    pip install -r requirements.txt
    ```

4. Configure the PostgreSQL database in `inventory_system/settings.py`:
    ```py
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.postgresql',
            'NAME': 'inventory_management',
            'USER': 'postgres',
            'PASSWORD': 'admin',
            'HOST': 'localhost',
            'PORT': '5432',
        }
    }
    ```

5. Apply the migrations:
    ```sh
    python manage.py migrate
    ```

6. Run the development server:
    ```sh
    python manage.py runserver
    ```

7. Open your browser and navigate to `http://127.0.0.1:8000/` to see the application.

## Features

- User registration and login
- Dashboard for logged-in users
- Tailwind CSS for styling

## License

This project is licensed under the MIT License.