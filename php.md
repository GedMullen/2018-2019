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
* Sort the output in 3 by first name.
* Sort the output in 3 by DOB.
* List all employees whose DOB is 18/1/1962 (dates can be referenced as strings - WHERE birth_date = '1961-08-29')
* Who is the oldest employee?
* Who is the newest (most recently hired) employee?
* List all female employees that were born in the 60s.
* List all male employees that were hired in the 80s.


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

