## Buidling Student Database - Part 1

Creating a Bash script that uses SQL to enter information about your Computer Science Students Database into PostgreSQL.

The students database includes four tables
* students table - columns include:
  * student_id - primary key
  * first_name
  * last_name
  * major_id - foreign key
  * gpa
* majors table - columns include:
  * major_id - primary key
  * major
* courses table - columns include:
  * course_id - primary key
  * course
* majors_courses table - columns include:
  * major_id 
  * course_id
  * composite key - major_id and course_id

### ====================== Files ========================
* students.csv
* courses.csv
* students.sql
* insert_data.sh

### Created a dump of all the commands for the inserting the data into the database
The command for the dump as a _"__students.sql__"_::
  * pg_dump --clean --create --inserts --username=freecodecamp students > students.sql
