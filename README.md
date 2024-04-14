# python-api

App using Python, Flask, Marshmallow to boostrap an api
https://auth0.com/blog/developing-restful-apis-with-python-and-flask/#-span-id--bootstrapping-flask----span--Bootstrapping-a-Flask-Application

# start the cashman application

./bootstrap.sh &

# get incomes

curl http://localhost:5000/incomes

# add new income

curl -X POST -H "Content-Type: application/json" -d '{
"description": "band gig",
"amount": 1000.0
}' http://localhost:5000/incomes
