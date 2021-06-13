# Exercise 4

- Run the following SQL statements to insert some data into each of your tables.

```
INSERT INTO customers (name, email, address, city, postcode, country) VALUES ('John Smith','j.smith@johnsmith.org','11 New Road','Liverpool','L10 2AB','UK');
INSERT INTO hotels (name, rooms, postcode) VALUES ('Triple Point Hotel', 10, 'CM194JS');
INSERT INTO bookings (customer_id, hotel_id, checkin_date, nights) VALUES (1, 1, '2019-10-01', 2);
```

- Run the 3 SQL statements above.
- Connect to your database and ensure the expected records have been created.
- Insert yourself in the customers table.
- Insert the following 3 hotels in the hotels table:
    - The Triple Point Hotel has 10 rooms, its postcode is CM194JS
    - The Royal Cosmos Hotel has 5 rooms, its postcode is TR209AX
    - The Pacific Petal Motel has 15 rooms, its postcode is BN180TG
- Try to insert a booking for a customer id which does not exist in the customers table (for example ID 100). What is happening and why?
- Use the following SQL statement to check that data has been correctly saved: `SELECT * FROM <table_name>;`
