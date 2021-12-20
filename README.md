# SampleAPIProject

## Setting up the database

```
python create_db.py
```

## Running Flask App 

Go to terminal and CD into the project directory
```
set FLASK_APP=main.py
set FLASK_ENV=development
flask run
```

## API Info

|HTTP Methods| URI | Actions |
|------------|-----|---------|
|GET|http://[hostname]/customers|Retrieve list of customers|
|GET|http://[hostname]/customers/[cust_id]|Retrieve a customer|
|POST|http://[hostname]/customers|Create a new customer|
|PUT or PATCH|http://[hostname]/customers/[cust_id]|Update an existing customer|
|DELETE|http://[hostname]/customers/[cust_id]|Delete a customer|

## Testing API requests

```python
import requests 
requests.get('http://127.0.0.1:5000/customers').json()  # GET list of all customers
```

All other requests can be tested using `call_api.py` as a reference.
