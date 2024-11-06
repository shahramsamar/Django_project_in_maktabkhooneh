# Django Project in Maktabkhooneh

A Django-based web application developed as part of the Maktabkhooneh learning project. This project demonstrates core Django features including user authentication, data management, and web interface design. It is designed to serve as a learning resource for building real-world applications with Django.

## Features

- **User Authentication**: Allows users to register, log in, and manage their profiles.
- **CRUD Operations**: Create, read, update, and delete records for models in the application.
- **Admin Panel**: Admins can manage all user data, settings, and other resources directly from the Django admin panel.
- **Forms**: Dynamic forms for submitting data through the web interface.
- **Responsive Design**: A simple and clean UI that adjusts to different screen sizes.

## Requirements

- **Python 3.x**
- **Django**: The main framework used to build this application.
- **PostgreSQL** (or another database system): The database used for storing application data.

### Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/shahramsamar/Django_project_in_maktabkhooneh.git
    cd Django_project_in_maktabkhooneh
    ```

2. **Install Dependencies:**

    If you're using `pip`, run:

    ```bash
    pip install -r requirements.txt
    ```

3. **Set up the Database**:

    Update the `settings.py` file to configure your database connection. For PostgreSQL:

    ```python
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.postgresql',
            'NAME': 'maktabkhooneh_db',
            'USER': 'your_db_user',
            'PASSWORD': 'your_db_password',
            'HOST': 'localhost',
            'PORT': '5432',
        }
    }
    ```

4. **Apply Migrations**:

    Run the following command to apply the database migrations:

    ```bash
    python manage.py migrate
    ```

5. **Create a Superuser (Admin)**:

    To create an admin user to access the Django admin panel:

    ```bash
    python manage.py createsuperuser
    ```

6. **Run the Development Server**:

    Start the development server with:

    ```bash
    python manage.py runserver
    ```

    The application will be accessible at `http://127.0.0.1:8000/`.

### How to Use

- **User Registration**: Register as a new user to access protected areas of the site.
- **User Login**: After registration, you can log in to the platform using your credentials.
- **CRUD Operations**: Perform CRUD operations on the resources available in the application (e.g., data entries).
- **Admin Panel**: Admin users can access the admin panel at `http://127.0.0.1:8000/admin/` to manage data.

### Project Structure

- `maktabkhooneh/`: Main Django app containing the core functionality of the application.
    - `models.py`: Contains the database models for the application.
    - `views.py`: Handles the logic behind rendering pages and processing user input.
    - `forms.py`: Defines forms used in the application.
    - `urls.py`: URL routing for the application.
    - `templates/`: Contains HTML templates for rendering views.
    - `static/`: Stores static files such as CSS, images, and JavaScript.
- `requirements.txt`: Lists all the dependencies needed for the project.
- `manage.py`: The main Django management script for running the project.

### Contributing

Feel free to fork the project and submit pull requests for new features, improvements, or bug fixes.

### License

This project is open-source and available for educational purposes.

---

This `README.md` provides detailed instructions on setting up, using, and contributing to the **Django Project in Maktabkhooneh**. It covers all the necessary setup and usage information for this Django-based application.

