# SciCommons Backend

This is the backend part of the SciCommons project, built with Django. It handles all the server-side logic, database interactions, and API endpoints for the application.


## Tech Stack

- **Framework:** Django
- **Database:** PostgreSQL (or any other database of your choice)
- **API:** Django REST Framework
- **MediaStorage** AWS s3

## Getting Started

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)
- Virtual environment (optional but recommended)

## Creating .env file
 
Make a .env file with following variables:

        EMAIL_HOST_USER = 
        EMAIL_HOST_PASSWORD = 
        EMAIL_PORT = 
        EMAIL_USE_TLS = 
        DEFAULT_FROM_EMAIL = 
        AWS_ACCESS_KEY_ID = 
        AWS_SECRET_ACCESS_KEY = 
        AWS_STORAGE_BUCKET_NAME = 
        AWS_S3_SIGNATURE_NAME = 
        AWS_S3_REGION_NAME = 
        AWS_S3_FILE_OVERWRITE = 
        AWS_DEFAULT_ACL =  
        AWS_S3_VERITY = 
        DEFAULT_FILE_STORAGE =
        DBNAME = 
        DBUSER =
        DBPASSWORD = 
        DBHOST = 
        DBPORT = 
        DATABASE_URL =

- Use DATABASE_URL, or default database based on your database connections.
- Add aws s3 bucket configuration for media file storage.
- Generate App Password for mail to use it for mail services.
- Note: Google has disabled the use of less secure apps, so you need to enable it to use the mail services. Go to this [link](https://myaccount.google.com/apppasswords) to generate the app password and place the password in the EMAIL_HOST_PASSWORD field.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/m2b3/SciCommons-backend
   cd SciCommons-backend
    ```

2. Create a virtual environment and activate it:
    ```bash
        python -m venv venv
        source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```
3. Install the required packages:

```bash
    pip install -r requirements.txt
```

4. Apply the migrations:

```bash
    python manage.py migrate
```

5. Create a superuser:
```bash
    python manage.py createsuperuser
```

6. Run the development server:
```bash
    python manage.py runserver
```

The backend server should now be running on http://localhost:8000.

## [GSOC REPORT](https://gist.github.com/JyothiSwaroopReddy07/89c56164a48a833e2bfdc8a5256c46d1)

## API Documentation
You can access the API documentation and interact with the available endpoints by visiting http://localhost:8000/docs when the development server is running.
You can see the documentation in swagger.

## Contributing
Contributions are always welcome! Please read the contribution guidelines first.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contact
If you have any questions or want to reach out to the team, please [create an issue](https://github.com/m2b3/SciCommons-backend/issues) on GitHub.

Made with :heart: by the SciCommons team
