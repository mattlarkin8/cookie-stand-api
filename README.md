# **LAB - Class 34**

## **Project: Back End Development**

### Author: Matthew Larkin

### Links

Live site deployed on Heroku: `https://larkin-cookie-stands.herokuapp.com/`

### Setup

Install dependencies from `requirements.txt`.

Use `python manage.py runserver` to test the site deployment on your local machine.

If you have docker, use `docker-compose up --build` to build and test a Docker deployment of the Django app.

### ENV

SECRET_KEY={your-secret-key}
DEBUG={True/False}
ALLOWED_HOSTS={localhost or deployed site}
ALLOW_ALL_ORIGINS={True/False}
DATABASE_ENGINE=django.db.backends.postgresql
DATABASE_NAME={your-db-name}
DATABASE_USER={your-db-user}
DATABASE_PASSWORD={your-db-PW}
DATABASE_HOST={your-db-url}
DATABASE_PORT={your-db-port}

### Tests

#### Deployment

Try setting up your own deployed environment and see if everything works fine. You should only need to make minimal changes to get it working, one very important change being your `.env` file. You could also use the `api_tester.py` to verify everything is working, but you will need all the required info for the deployment you are testing.

#### HTTP Testing

Use ThunderClient or another HTTP client to test the API routes.

You should be able to:

- Get to the Snack List view at `http://localhost:8000/api/v1/cookie_stand/`. (Requires authentication token)
- Go to the Snack Detail view for any snack using its id. Ex: `http://localhost:8000/api/v1/cookie_stand/1/` (Requires authentication token)
- Obtain your token pair by going to `http://localhost:8000/api/token/`
- Refresh your access token by going to `http://localhost:8000/api/token/refresh`
