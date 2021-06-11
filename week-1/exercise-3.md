# Exercise 3

- open the postgres terminal with `psql`, and connect to your database using `\c cyf_hotels`
- Create the customers table in the `cyf_hotels` database.
- Verify that the table customers is created with the psql command `\dt` which lists the existing tables.
- Display the table customers definition with the command `\d customers` and verify that it matches what you expect.
- Create a new table hotels in the `cyf_hotels` database with the following columns: `id`, `name`, `number_of_rooms`, and `postcode`. Use the commands above to verify that the table is correctly created.


Now that we have a table to store customers and a table to store hotels, we can create a table to hold the bookings of customers for an hotel with the checkin date and the number of nights they intend to stay:

```
CREATE TABLE bookings (
  id               SERIAL PRIMARY KEY,
  customer_id      INT REFERENCES customers(id),
  hotel_id         INT REFERENCES hotels(id),
  checkin_date     DATE NOT NULL,
  nights           INT NOT NULL
);
```

In the above, `customer_id` and `hotel_id` are called foreign keys as they reference an id from a different table. This set a very strong constraint as you will not be able to create a booking for a customer id which does not exist in the customers table!

- Create the table bookings in your `cyf_hotels` database and verify that it is correctly created.
