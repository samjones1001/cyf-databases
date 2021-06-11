#Exercise 1

So far we know that information in a relational database is stored is *tables*, *columns*, and *rows*.

- The database itself represents a collection of all the information you want to store.
- The database contains one or more tables. Each table represents a collection of information about a particular object or piece of data which is important to your system.
- Each column in a table represents a particular attribute of the data stored there.
- Each row in a table represents a single record.

To think about a real world example, you might imagine a library as a database.
- The library might store many different types of objects in its collection. For example, books, magazines, newspapers and so on. Each of these types of object might be a table within your library database.
- For each category of item, you might want to store particular pieces of information. For example, for a book, you might need to store the author, title, and year of publication. Each of these pieces of information would be represented as columns in the book table.
- Each row in the book table would represent a particular book.

So, your book table might end up looking something like this:

|id|title|author|year_of_publication|
|:-:|:--:|:----:|:-----------------:|
|1  |Harry Potter and the Chamber of Secrets|J.K. Rowling|1998|
|2  |The Gruffalo|Julia Donaldson|1999|

Think about the following lists. Each list represents another real world example which we can imagine as a database. In each list, which element makes most sense as a table, a column, a row, and as the database itself?

## 1

- The courses run at a university
- The university itself
- A computer science course
- The number of students on a course

## 2

- Star Wars
- A cinema
- The screen number which a particular film is showing on
- The films being shown at the cinema

## 3

- The price of a vegetable
- All of the vegetables sold at a supermarket
- The supermarket itself
- A bag of carrots
