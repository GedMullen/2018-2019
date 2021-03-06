<!--
11 - more sql/php
12 - create a table
13 - form
14 - form answer
-->

# Week 16 & 17

* Set up the code for this week:
```bash
mkdir crudtutorial
cd crudtutorial
git clone https://github.com/GedMullen/php.git
cd php/week16/crud
```
* Update customers.sql with your database name and run the script to set up your database.
* Update database.php with your database name.

## Exercises

* Work your way through the [online CRUD tutorial](https://www.startutorial.com/articles/view/php-crud-tutorial-part-1).
* Use the tutorial code as a template to build a CRUD web application of your choice.

# Week 14

* [Google Fonts](https://www.w3schools.com/howto/howto_google_fonts.asp)
* [Regular Expressions](https://github.com/ziishaned/learn-regex)
* Set up Week 14 example code
```bash
mkdir forms
cd forms
git clone https://github.com/GedMullen/php.git
cd php/week14/example1
```

## Exercises

* Complete the following [exercises](https://docs.google.com/document/d/1NM3z7RhYvzyAaziHf1pInuv8Vdava2Swc4Ha7Nfi56s/edit?usp=sharing).


# Week 13

* Set up Week 13 example code
```bash
mkdir homepage
cd homepage
git clone https://github.com/GedMullen/php.git
cd php/week13/example1
```

## Exercises

* Complete the following [exercises](https://docs.google.com/document/d/1aSA95OAXIWO8xCH0uwZ5NrgiBxwYohv0zJGRQrpKsKs/edit?usp=sharing).

# Week 12

* [CSS Frameworks](https://hackernoon.com/top-5-most-popular-css-frameworks-that-you-should-pay-attention-to-in-2017-344a8b67fba1)
* [PHP Form Processing](https://www.w3schools.com/php/php_form_validation.asp)
* Set up Week 12 example code
```bash
mkdir loginexample
cd loginexample
git clone https://github.com/GedMullen/php.git
cd php/week12
```
* Follow the instructions in class to setup the database and run the application
```bash
mysql -h 104.154.XXX.65 -u student  < database.sql
php -S 0.0.0.0:8081
```

## Exercise

* Complete the [PHP Form Processing](https://www.w3schools.com/php/php_form_validation.asp) tutorial. Get the example working in cloud shell. 
* Modify menu.php to check if the username entered is correct.
* Add a password to the users table and check that the password is correct. 


## Week 11 Answers

```sql
SELECT count(*)
FROM employees
WHERE gender="F"
AND birth_date LIKE '%195%';

SELECT  salaries.emp_no
FROM salaries
ORDER BY salaries.salary DESC
LIMIT 1;

SELECT  salaries.*, employees.first_name, employees.last_name, employees.gender, employees.birth_date, employees.hire_date
FROM salaries
INNER JOIN employees
ON salaries.emp_no=employees.emp_no
ORDER BY salaries.salary DESC
LIMIT 1;

-- Simplified Inner Join example
SELECT  salaries.*, employees.first_name, employees.last_name, employees.gender, employees.birth_date, employees.hire_date
FROM salaries, employees
WHERE salaries.emp_no=employees.emp_no
ORDER BY salaries.salary ASC
LIMIT 1;

SELECT salaries.*, employees.first_name, employees.last_name, employees.gender, employees.birth_date
FROM salaries
INNER JOIN employees
ON salaries.emp_no=employees.emp_no
WHERE first_name="Berni"
AND last_name="Sanella"
AND birth_date="1961-08-29"
ORDER BY to_date;

SELECT s.salary * 0.1 AS Pension
        FROM salaries s, employees e
        WHERE s.emp_no=e.emp_no
        AND e.first_name = 'Berni'
        AND e.last_name = 'Sanella'
        AND e.birth_date = '1961-08-29';

SELECT salary/12 AS Salary
        FROM salaries s, employees e
        WHERE e.emp_no = s.emp_no
        AND from_date < '1997-10-01'
        AND to_date > '1997-10-31'
        AND first_name = 'Berni'
        AND last_name = 'Sanella'
        AND birth_date = '1961-08-29';
```

# Week 11

* [MySQLi examples](http://php.net/manual/en/mysqli.examples-basic.php)
* [index.php example code](https://github.com/GedMullen/php/blob/master/week11/index.php)
* Running example:
```bash
mkdir week11
cd week11
git clone https://github.com/GedMullen/php.git
cd php/week11
```
* Edit index.php with the correct IP address.
* Run a PHP webserver and view the output using Web View. Change the port to 8081. 
```bash
php -S 0.0.0.0:8081
```
* [Joins](http://www.w3schools.com/sql/sql_join.asp)
* [Aliases](https://www.w3schools.com/sql/sql_alias.asp)

## Exercises

* Create SQL for the following exercises and use PHP to output the results to a HTML table. 
* Count the number of female employees that were born in the 50s.
* What is the employee id of the person with the highest salary?
* Find the employee details (name DOB etc) of the person with the highest salary (you will need to join the salaries and employees tables).
* Find the employee details of the person with the lowest salary.
* List all the salaries of Berni Sanella DOB 29/8/61 - order the query by to_date;
* Create an alias for the pension column in Q5 called “Pension”.
* How much was Bernie paid in the month of October 1997 ( salary / 12 )?



# Week 10

* MySQL manual page:
```
man mysql
```
* Using MySQL interactively:
```
mysql -h 104.154.XXX.65 -u student employees 
```
* Useful MySQL commands:
```
SHOW TABLES;
DESCRIBE employees;
```
* Connecting to MySQL and running a PHP server
```bash
mkdir week10
cd week10
git clone https://github.com/GedMullen/php.git
cd php/intro
```
* Edit index.php with the correct IP address.
* Run a PHP webserver and view the output using Web View. Change the port to 8081. 
```bash
php -S 0.0.0.0:8081
```

## Exercises
* Familiarise yourself with the man pages for the mysql command.
* Run some of the SQL scripts you created in week 9 interactively.  
* Create an index.php page that displays the output from the SQL you created in week 9 to the browser. Use [HTML Tables](https://www.w3schools.com/html/html_tables.asp) to do this. Add CSS to format the tables. 

# Week 9

* [MySQL Example Employee Database](https://dev.mysql.com/doc/employee/en/sakila-structure.html)
```
mkdir sqlexercises
cd sqlexercises
```
* Create a file called week9.sql and add the following line:
```sql
SELECT * FROM employees LIMIT 10;
```
* Run your SQL script using the following command:
```
mysql -h 104.154.XXX.65 -u student employees < week9.sql
```
* [Select](http://www.w3schools.com/sql/sql_select.asp)
* [Where](http://www.w3schools.com/sql/sql_where.asp)
* [Order By](http://www.w3schools.com/sql/sql_orderby.asp)
* [Count](https://www.w3schools.com/sql/sql_count_avg_sum.asp)
* [And & Or](http://www.w3schools.com/sql/sql_and_or.asp)
* [Dates](http://www.w3schools.com/sql/sql_dates.asp) 

## Exercises

* Create an SQL script in your sqlexercises folder called week9.sql and write a SELECT statement that outputs a list of the first 10 female employees (use LIMIT 10). Append the following exercises to your script: 
* A list of female employees that have a last name of “Gils”
* Use the SQL created in Exercise 2 to create a list showing only the first name, last name and DOB.
* Sort the output in previous question by first name.
* Sort the output in previous question by DOB.
* List all employees whose DOB is 18/1/1962 (dates can be referenced as strings - WHERE birth_date = '1961-08-29')
* Who is the oldest employee?
* Who is the newest (most recently hired) employee?
* List all female employees that were born in the 60s.
* List all male employees that were hired in the 80s.

### Answers

```sql
SELECT * 
FROM employees 
WHERE gender="F" 
LIMIT 10; 

SELECT * 
FROM employees 
WHERE gender="F" 
AND last_name="Gils"
LIMIT 10; 

SELECT first_name, last_name, birth_date  
FROM employees
WHERE last_name="Gils"
AND gender="F" 
LIMIT 10;

SELECT first_name, last_name, birth_date  
FROM employees
WHERE last_name="Gils"
AND gender="F"
ORDER BY first_name 
LIMIT 10;

SELECT first_name, last_name, birth_date  
FROM employees
WHERE last_name="Gils"
AND gender="F"
ORDER BY birth_date 
LIMIT 10;

SELECT * 
FROM employees 
WHERE birth_date="1962-01-18"
LIMIT 10;

SELECT first_name, last_name, birth_date 
FROM employees 
ORDER BY birth_date ASC 
LIMIT 1; 

SELECT first_name, last_name, birth_date 
FROM employees 
ORDER BY hire_date ASC 
LIMIT 1; 

SELECT first_name, last_name, hire_date 
FROM employees 
WHERE gender='F'
AND birth_date BETWEEN '1960-01-01' and '1969-12-31' 
ORDER BY birth_date
LIMIT 10;

-- Solution using LIKE
SELECT first_name, last_name, hire_date 
FROM employees 
WHERE gender="M" 
AND hire_date LIKE '%198%' 
ORDER BY hire_date ASC
LIMIT 10;

```


# Week 8

* [PHP Documentation](http://www.php.net/)
* [PHP Tutorial](http://www.w3schools.com/php/) 

# Exercise

* Implement this [PHP script](https://www.w3schools.com/php/) in Google Cloud.

# Week 7

* [Octoverse Trends](https://octoverse.github.com/projects.html)
* [Why is JavaScript So Popular?](https://www.simplytechnologies.net/blog/2018/4/11/why-is-javascript-so-popular)
* [HTML with JavaScript](https://www.w3schools.com/html/html_scripts.asp)
* [JavaScript Examples](https://www.w3schools.com/js/js_examples.asp)
* [Eloquent JavaScrtipt](https://github.com/marijnh/Eloquent-JavaScript)
* [JavaScript Style Guide](https://github.com/airbnb/javascript)
* [Codecademy JavaScript](https://www.codecademy.com/learn/introduction-to-javascript)

# Exercise

* Expand the functionality of your websites using the [JavaScript Examples](https://www.w3schools.com/js/js_examples.asp).

<!--
* [HTML Timeline](https://www.w3schools.com/Html/html5_intro.asp)
* [HTML DOM Tree](https://www.w3schools.com/js/js_htmldom.asp)
* [Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools/css/) 
-->

# Week 6

* [Example Webpage](https://gist.github.com/Haxoras/7990467)
* [Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools/css/) 
<!--
* [JavaScript Examples](https://www.w3schools.com/js/js_examples.asp)
* [JavaScript Tutorial](https://www.w3schools.com/js/)
-->

# Week 5

* [More CSS](https://drive.google.com/file/d/1NQM0xI_vUf0zp6xtQUrhhSteYdnYJAbB/view?usp=sharing)

## Exercises

* Continue to develop your informative website using the CSS style you chose from last week. 

# Week 4

* [CSS Tutorial](https://www.w3schools.com/Css/)
* [CSS Zen Garden](http://csszengarden.com/)
* [Example Design](http://www.csszengarden.com/175/)
* [JTechnologies](http://www.jtechnologies.co.uk/)

## Exercise

* Pick a subject for an informative website and find a design that matches your chosen subject from the [CSS Zen Garden](http://csszengarden.com/).
* Download the required HTML, CSS and images so that your chosen design renders on your computer.
* Use the design as a template to create your own informative web page.  

# Week 3 

* [Web Architecture](https://docs.google.com/presentation/d/1ERXT_L5CjzsJ6gce4kjpXQ5wPi54dAmRqJNUWFGMHX4/edit?usp=sharing)
* [w3schools HTML Tutorial](https://www.w3schools.com/html/default.asp) 
* [Notepad ++](https://notepad-plus-plus.org/)
* [Cloud Shell](https://console.cloud.google.com/cloudshell/)
## Exercises

* Follow [this brief](https://docs.google.com/document/d/1jmYj8g8ai9_kYZ5EtyEAa6BsLbkjKG6TsLn4n8j67b8/edit?usp=sharing)

# Week 2

* [Dynamically Generated Content](https://docs.google.com/presentation/d/1bWMd9ypXXUJGt-jDpjpRSfh6_2zHMRKjjBcldO0OMeM/pub?start=false&loop=false&delayms=60000&slide=id.p10)
* [Netcraft Survey](https://news.netcraft.com/archives/2018/07/19/july-2018-web-server-survey.html)

## Exercise

* Complete the [Learning the Command Line on Codecademy](https://www.codecademy.com/learn/learn-the-command-line) course.

# Week 1

* Unit descriptors [ Developing Websites for Multiplatform Use](http://www.mysqa.info/files/hn/H1J935.pdf) and [Web Development: Essential Content](https://www.sqa.org.uk/files/hn/HF5834.pdf)
* [Corners Game](https://docs.google.com/document/d/1f8YCnRpKR5dgO-aP77ZXJg5SU6BWLMkiLsc99n1WZe4/pub)
* [Getting Started With Cloud Shell](https://cloud.google.com/shell/docs/starting-cloud-shell)
* [GitHub Is Your New CV](http://code.dblock.org/2011/07/14/github-is-your-new-resume.html)
* [GitHub Home](https://github.com/)
* [Example Profile](https://github.com/marijnh)
* Running the example code in Cloud Shell:
```bash
mkdir week1
cd week1
git clone https://github.com/GedMullen/php.git
cd php/intro
```
* Edit index.php with the correct IP address.
* Run a PHP webserver and view the output using Web View. Change the port to 8081. 
```bash
php -S 0.0.0.0:8081
```

## Exercises

* Complete the [Getting Started With Cloud Shell](https://cloud.google.com/shell/docs/starting-cloud-shell) tutorial. You will need a google account for this.
* Create a GitHub accound and Complete these [GitHub Exercises](https://docs.google.com/document/d/1lYOmyY0liBNXntOP9yipcD7Cy-aqKqAU1gkrSmdd2e4/edit?usp=sharing)

