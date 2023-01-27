## Buidling Student Database - Part 1

Creating a Bash script that uses SQL to enter information about your Computer Science Students Database into PostgreSQL.

### +++++++++++++++++++ Files +++++++++++++++++
* students.csv
* courses.csv
* students.sql
* insert_data.sh

# Created a dump of all the commands for the inserting the data into the database
The command for the dump as a "students.sql"::
  pg_dump --clean --create --inserts --username=freecodecamp students > students.sql
