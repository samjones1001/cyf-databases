# Exercise 4

- Try running each of the following SQL statements in your psql promt. Discuss them as a group and try to understand what each is doing.

```
SELECT A.column1, B.column2 FROM A INNER JOIN B ON A.b_id=B.id;
```

```
SELECT * FROM customers INNER JOIN bookings ON customers.id=bookings.customer_id;
```

```
SELECT * FROM bookings
INNER JOIN customers ON customers.id=bookings.customer_id
INNER JOIN hotels ON hotels.id=bookings.hotel_id;
```

```
SELECT bookings.checkin_date,customers.name,hotels.name FROM bookings
INNER JOIN customers ON customers.id=bookings.customer_id
INNER JOIN hotels ON hotels.id=bookings.hotel_id
WHERE customers.id=1;
```

- Retrieve all the bookings along with customer data for bookings starting in 2020
- Retrieve the customer names, booking start dates and number of nights for all customers who booked the hotel name Jade Peaks Hotel
- Retrieve all the booking start dates with customer names and hotel names for all bookings for more than 5 nights
