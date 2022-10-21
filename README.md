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
Python -m venv env
(For Mac) source env/bin/activate
(For Windows) env/Scripts\activate
pip install -r requirements.txt
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
# Open http://127.0.0.1:8000/posts/

# To have dummy data for testing run:
python manage.py fixtures/dummy-data.json
```

3. Frontend setting

```
cd frontend
npm install
npm start
# Open http://127.0.0.1:3000/
```
