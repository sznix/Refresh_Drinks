# Refresh Drinks in React & Redux + Django

```
Refresh Drinks, with a frontend built in React & Redux and a backend built in Django API.
This is a mini e-commerce project designed to help promote sales of refreshments. And a great
way to stay refreshed this summer is by ordering refreshing lemonades with a single zesty click!
The project introduces a fresh and exciting way to sell lemonades in different flavors! Designed
to save users from commute time and expenses by placing your orders from the comfort of their homes.
```

## Live Demo

**This App uses a Heroku free plan, so I am afraid that it takes time to load the pages.**

Check out [FRONTEND LIVE DEMO](https://refresh-drinks-frontend.sznix.repl.co) here!!

Check out [API LIVE DEMO](https://refresh-drinks-backend.sznix.repl.co) here!!

## Tech used

```
* Frontend : React & Redux
* Backend : Django
```

## How to Install

1. Git Clone

```
git clone git@github.com:sznix/Refresh_Drinks.git
```

2. Backend setting

```
cd backend

# Create and activate virtual environment
Python -m venv env
(For Mac) source env/bin/activate
(For Windows) env/Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Configure environment variables
# Copy .env.example to .env and update with your credentials
cp .env.example .env
# Edit .env file with your actual credentials

# Run migrations
python manage.py makemigrations
python manage.py migrate

# Start the server
python manage.py runserver
# Open http://127.0.0.1:8000/posts/

# To have dummy data for testing run:
python manage.py loaddata fixtures/dummy-data.json
```

**Security Note**: Never commit the `.env` file with actual credentials. The `.env.example` file is provided as a template.

3. Frontend setting

```
cd frontend
npm install
npm start
# Open http://127.0.0.1:3000/
```

## Security Configuration

This application uses environment variables to protect sensitive credentials. The following security improvements have been implemented:

### Environment Variables

All sensitive configuration values should be set via environment variables:

- **SECRET_KEY**: Django secret key for cryptographic signing
- **DEBUG**: Set to `False` in production
- **ALLOWED_HOSTS**: Comma-separated list of allowed hostnames
- **CORS_ALLOW_ALL_ORIGINS**: Set to `False` in production
- **Database credentials**: DB_NAME, DB_USER, DB_PASSWORD, DB_HOST, DB_PORT
- **Cloudinary credentials**: CLOUDINARY_CLOUD_NAME, CLOUDINARY_API_KEY, CLOUDINARY_API_SECRET

### Setup for Development

1. Copy the `.env.example` file in the backend directory to `.env`
2. Update the values in `.env` with your actual credentials
3. Never commit the `.env` file to version control

### Setup for Production

Set environment variables in your hosting platform (Heroku, AWS, etc.) with production values. Ensure:
- DEBUG is set to False
- SECRET_KEY is a strong, random value
- ALLOWED_HOSTS includes only your production domain(s)
- CORS_ALLOW_ALL_ORIGINS is False (or configure specific allowed origins)
- All credentials use production values

