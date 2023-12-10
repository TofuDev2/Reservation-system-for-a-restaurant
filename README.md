# Reservation-system-for-a-restaurant
This is a final project for subject python i learned in University

## Installation Requirements
Simple restaurant reservation system built in Flask & Python application requires Flask, the Flask SQL Alchemy extension

Flask:
```
pip install Flask
```

Flask SQL Alchemy
```
pip install Flask-SQLAlchemy
```

WTForms
```
pip install WTForms
```

## Running the application
Simply run "run.py", this will start the local web server.

## Admin section
To access the admin portion of the application, go to /admin.
## Table design
Guest
* ID - Primary Key
* name - String
* phone_number - String

Table
* ID - Primary Key 
* Capacity - Integer

Reservation
* ID - Primary Key
* guest_id - Foreign Key(Guest)
* table_id - Foreign Key(Table)
* num_guests - Integer
* reservation_time - DateTime
## Misc
Assumed reservation length - 1 hour (see app/models.py)
Restaurant opening time - 4pm
Restaurant closing time - 10pm (see app/views.py)
