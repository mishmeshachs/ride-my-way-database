# ride-my-way-database
[![Build Status](https://travis-ci.org/mishmeshachs/ride-my-way-database.svg?branch=developer)](https://travis-ci.org/mishmeshachs/ride-my-way-database)
[![Coverage Status](https://coveralls.io/repos/github/mishmeshachs/ride-my-way-database/badge.svg?branch=developer)](https://coveralls.io/github/mishmeshachs/ride-my-way-database?branch=developer)

 Web Application that enable users(CarTax Operators) to create an account and be able to create ride offers. Passengers will be able to view the ride offers and request to join:

- Register an account and Login into it.
- Register, Update and delete a Ride .
- View all Rides.
- View One Rides.
- Post Requests for rides.
- View all Requests for rides
- Accept a ride request
- Reject a ride request
- Delete a ride offer
- Delete a ride request
- Update a ride offer
- Update a request for a ride

## Prerequisites

- Python 3.6 or a later version

## Installation
Clone the repo.
```
$ git clone https://github.com/mishmeshachs/ride-my-way-database-.git
```
and cd into the folder:
```
$ /Ride-My-Way3-
```
## Virtual environment
Create a virtual environment:
```
$ mkvirtualenv <virtual environment name>
```
## Dependencies
Install package requirements to your environment.
```
pip install -r requirements.txt
```

## Database Setup

$ python create_tables.py
```

## Testing

To set up unit testing environment:

```
$ pip install nose
$ pip install coverage
```

To run tests perform the following:

```
$ nosetests --with-coverage. Also pytest -v
```


##Start The Server
To start the server run the following command
```
Then run:
python run.py 
```
The server will run on port: 5000

## Testing API on Postman




### API endpoints
| Endpoint | Method |  Functionality | Authentication |
| --- | --- | --- | --- |
| /api/auth/v2/register | POST | Creates a user account | FALSE
| /api/auth/v2/login | POST | Logs in a user | TRUE
| /api/v2/rides | POST | Creates a ride | TRUE
| /api/v2/rides | GET | Retrieves all rides | TRUE 
| /api/v2/rides/{ride_id} | GET | Get a ride | TRUE
| /api/v2/rides/{ride_id} | PUT | Update a ride details | TRUE
| /api/v2/rides/{ride_id} | DELETE | Delete a ride | TRUE
| /api/v2/rides/{ride_id}/requests | POST | Request a ride | TRUE
| /api/v2/rides/requests | GET | Get all requests for rides | TRUE
| /api/v2/rides/requests/{request_id} | GET | Get a single request | TRUE
| /api/v2/rides/requests/{request_id} | PUT | Update a single request | TRUE
| /api/v2/rides/requests/{request_id} | DELETE | Delete a single request | TRUE
| /api/v2/rides/requests/accept{request_id} | PUT | Accept a request | TRUE
| /api/v2/rides/requests/reject{request_id} | PUT | Reject a request | TRUE

## API Documentation
