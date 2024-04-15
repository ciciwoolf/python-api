# python-api

I've built a simple REST api app using Python, a framework called Flask, Marshmallow.

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
