# SQL Homework

The Springfield Cinema is having a Marvel Movie Marathon! They have asked you to help maintain their database of movies with times and attendees.

## To access the database:

First, create a database called 'marvel'

```
# terminal
createdb marvel
```

Next, run the provided SQL script to populate your database:

```
# terminal
psql -d marvel -f marvel.sql
```

Use the supplied data as the source of data to answer the questions. Copy the SQL command you have used to get the answer, and paste it below the question, along with the result they gave.

## Questions

1.  Return ALL the data in the 'movies' table.

id |                title                | year | show_time
----+-------------------------------------+------+-----------
 1 | Iron Man                            | 2008 | 17:00
 2 | The Incredible Hulk                 | 2008 | 23:55
 3 | Iron Man 2                          | 2010 | 18:45
 4 | Thor                                | 2011 | 15:45
 5 | Captain America: The First Avenger  | 2011 | 14:15
 6 | Avengers Assemble                   | 2012 | 14:45
 7 | Iron Man 3                          | 2013 | 21:55
 8 | Thor: The Dark World                | 2013 | 22:55
 9 | Batman Begins                       | 2005 | 13:40
10 | Captain America: The Winter Soldier | 2014 | 18:25
11 | Guardians of the Galaxy             | 2014 | 13:10
12 | Avengers: Age of Ultron             | 2015 | 20:20
13 | Ant-Man                             | 2015 | 13:00
14 | Captain America: Civil War          | 2016 | 12:35
15 | Doctor Strange                      | 2016 | 22:00
16 | Guardians of the Galaxy 2           | 2017 | 14:05
17 | Spider-Man: Homecoming              | 2017 | 23:00
18 | Thor: Ragnarok                      | 2017 | 22:10
19 | Black Panther                       | 2018 | 21:00

2.  Return ONLY the name column from the 'people' table

name         
----------------------
Homer Simpson
Marge Simpson
Lisa Simpson
Maggie Simpson
Patty Bouvier
Selma Bouvier
Kent Brockman
Ned Flanders
Barney Gumble
Itchy
Eric Cartman
Scratchy
Crusty the Clown
Montgomery Burns
Mayor Joe Quimby
Groundskeeper Willie

3.  Oops! Someone spelled Krusty The Klown's name wrong! Change it to reflect the proper spelling (Crusty should be Krusty).

id |         name         
----+----------------------
 1 | Homer Simpson
 2 | Marge Simpson
 3 | Lisa Simpson
 4 | Maggie Simpson
 5 | Patty Bouvier
 6 | Selma Bouvier
 7 | Kent Brockman
 8 | Ned Flanders
 9 | Barney Gumble
10 | Itchy
11 | Eric Cartman
12 | Scratchy
14 | Montgomery Burns
15 | Mayor Joe Quimby
16 | Groundskeeper Willie
13 | Krusty the Clown

4.  Return ONLY Homer Simpson's name from the 'people' table.

name      
---------------
Homer Simpson

5.  The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.

id |                title                | year | show_time
----+-------------------------------------+------+-----------
 1 | Iron Man                            | 2008 | 17:00
 2 | The Incredible Hulk                 | 2008 | 23:55
 3 | Iron Man 2                          | 2010 | 18:45
 4 | Thor                                | 2011 | 15:45
 5 | Captain America: The First Avenger  | 2011 | 14:15
 6 | Avengers Assemble                   | 2012 | 14:45
 7 | Iron Man 3                          | 2013 | 21:55
 8 | Thor: The Dark World                | 2013 | 22:55
10 | Captain America: The Winter Soldier | 2014 | 18:25
11 | Guardians of the Galaxy             | 2014 | 13:10
12 | Avengers: Age of Ultron             | 2015 | 20:20
13 | Ant-Man                             | 2015 | 13:00
14 | Captain America: Civil War          | 2016 | 12:35
15 | Doctor Strange                      | 2016 | 22:00
16 | Guardians of the Galaxy 2           | 2017 | 14:05
17 | Spider-Man: Homecoming              | 2017 | 23:00
18 | Thor: Ragnarok                      | 2017 | 22:10
19 | Black Panther                       | 2018 | 21:00

6.  We forgot one of the main characters! Add Bart Simpson to the 'people' table

id |         name         
----+----------------------
 1 | Homer Simpson
 2 | Marge Simpson
 3 | Lisa Simpson
 4 | Maggie Simpson
 5 | Patty Bouvier
 6 | Selma Bouvier
 7 | Kent Brockman
 8 | Ned Flanders
 9 | Barney Gumble
10 | Itchy
11 | Eric Cartman
12 | Scratchy
13 | Crusty the Clown
14 | Montgomery Burns
15 | Mayor Joe Quimby
16 | Groundskeeper Willie
17 | Bart Simpson

7.  Eric Cartman has decided to hijack our movie evening, Remove him from the table of people.

id |         name         
----+----------------------
 1 | Homer Simpson
 2 | Marge Simpson
 3 | Lisa Simpson
 4 | Maggie Simpson
 5 | Patty Bouvier
 6 | Selma Bouvier
 7 | Kent Brockman
 8 | Ned Flanders
 9 | Barney Gumble
10 | Itchy
12 | Scratchy
13 | Crusty the Clown
14 | Montgomery Burns
15 | Mayor Joe Quimby
16 | Groundskeeper Willie
(15 rows)


8.  The cinema has just heard that they will be holding an exclusive midnight showing of 'Avengers: Infinity War'!! Create a new entry in the 'movies' table to reflect this.

id |                title                | year | show_time
----+-------------------------------------+------+-----------
  1 | Iron Man                            | 2008 | 17:00
  2 | The Incredible Hulk                 | 2008 | 23:55
  3 | Iron Man 2                          | 2010 | 18:45
  4 | Thor                                | 2011 | 15:45
  5 | Captain America: The First Avenger  | 2011 | 14:15
  6 | Avengers Assemble                   | 2012 | 14:45
  7 | Iron Man 3                          | 2013 | 21:55
  8 | Thor: The Dark World                | 2013 | 22:55
  9 | Batman Begins                       | 2005 | 13:40
 10 | Captain America: The Winter Soldier | 2014 | 18:25
 11 | Guardians of the Galaxy             | 2014 | 13:10
 12 | Avengers: Age of Ultron             | 2015 | 20:20
 13 | Ant-Man                             | 2015 | 13:00
 14 | Captain America: Civil War          | 2016 | 12:35
 15 | Doctor Strange                      | 2016 | 22:00
 16 | Guardians of the Galaxy 2           | 2017 | 14:05
 17 | Spider-Man: Homecoming              | 2017 | 23:00
 18 | Thor: Ragnarok                      | 2017 | 22:10
 19 | Black Panther                       | 2018 | 21:00
 20 | Avengers: Infinity War              |      |
(20 rows)

9.  The cinema would like to make the Iron Man movies a triple billing. Find out the show time of "Iron Man 2" and set the show time of "Iron Man 3" to start two hours later.

show_time
-----------
 18:45

 UPDATE 1
  id |         name         
 ----+----------------------
   1 | Homer Simpson
   2 | Marge Simpson
   3 | Lisa Simpson
   4 | Maggie Simpson
   5 | Patty Bouvier
   6 | Selma Bouvier
   7 | Kent Brockman
   8 | Ned Flanders
   9 | Barney Gumble
  10 | Itchy
  11 | Eric Cartman
  12 | Scratchy
  13 | Crusty the Clown
  14 | Montgomery Burns
  15 | Mayor Joe Quimby
  16 | Groundskeeper Willie
 (16 rows)

  id |                title                | year | show_time
 ----+-------------------------------------+------+-----------
   1 | Iron Man                            | 2008 | 17:00
   2 | The Incredible Hulk                 | 2008 | 23:55
   3 | Iron Man 2                          | 2010 | 18:45
   4 | Thor                                | 2011 | 15:45
   5 | Captain America: The First Avenger  | 2011 | 14:15
   6 | Avengers Assemble                   | 2012 | 14:45
   8 | Thor: The Dark World                | 2013 | 22:55
   9 | Batman Begins                       | 2005 | 13:40
  10 | Captain America: The Winter Soldier | 2014 | 18:25
  11 | Guardians of the Galaxy             | 2014 | 13:10
  12 | Avengers: Age of Ultron             | 2015 | 20:20
  13 | Ant-Man                             | 2015 | 13:00
  14 | Captain America: Civil War          | 2016 | 12:35
  15 | Doctor Strange                      | 2016 | 22:00
  16 | Guardians of the Galaxy 2           | 2017 | 14:05
  17 | Spider-Man: Homecoming              | 2017 | 23:00
  18 | Thor: Ragnarok                      | 2017 | 22:10
  19 | Black Panther                       | 2018 | 21:00
   7 | Iron Man 3  

## Extension

1.  Research how to delete multiple entries from your table in a single command.


DELETE FROM table WHERE col1='4' and col2='5'

DELETE FROM table WHERE col1 IN (1,2,3,4,5)
