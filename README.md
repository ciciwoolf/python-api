# python-api

A simple REST api app using Python, a framework called Flask, and a datatype library called Marshmallow. Code is based on this tutorial:

https://auth0.com/blog/developing-restful-apis-with-python-and-flask/#-span-id--bootstrapping-flask----span--Bootstrapping-a-Flask-Application

## start the cashman application

```
./bootstrap.sh &
```

## get expenses

```
curl http://localhost:5000/expenses
```

## add a new expense

```
curl -X POST -H "Content-Type: application/json" -d '{
    "amount": 20,
    "description": "lottery ticket"
}' http://localhost:5000/expenses
```

## get incomes

```
curl http://localhost:5000/incomes
```

## add new expenses

```
curl -X POST -H "Content-Type: application/json" -d '{
    "amount": 300.0,
    "description": "loan payment"
}' http://localhost:5000/incomes
```

# Docker

## build Docker image

```
docker build -t cashman .
```

## run a new docker container named cashman

```
docker run --name cashman \
    -d -p 5000:5000 \
    cashman
```
