Setup:
Cd into Airline_API
Run: python manage.py runserver

Information about the database:

There are only 5 flights available:
E15	2023-06-10 12:30:00	BCN	LGW
SA21	2023-06-17 12:30:00	LGW	BCN
LG12	2023-06-20 10:00:00	CDG	FCO
TD02	2023-06-15 17:00:00	FRA	AMS
UV32	2023-06-24 19:00:00	MAD	LGW

The following seat codes are are on each flight:
A1 Economy
A2 Economy
A3 Economy
A4 Economy
A5 Economy
A6 Economy
B1 Business
B2 Business
B3 Business

You can only cancel a booking if it is 48 hours before the departure date of the flight.


Here is an example of how to send an appropriate url:

1. http://sc20j2h.pythonanywhere.com/smash_airline/BCN/LGW/2023-06-10/Economy/1/0
2. http://sc20j2h.pythonanywhere.com/smash_airline/E15/A2
3. http://sc20j2h.pythonanywhere.com/booking/71 (put the booking id returned)
4. http://sc20j2h.pythonanywhere.com/smash_airline/booking/cancel/71 (put the booking id returned)
