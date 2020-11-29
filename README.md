# SQL_for_Data_Analysis
this project was about investigating a relational Sakila Movie database an online DVD rentals database using SQL for Data Analysis
***************************************************************************************************************************************************************
What are the Question Sets?
We have also provided a set of questions that you are free to consider and include in your Project Submission. These are solely provided for your convenience,
and you can choose to use any of the questions in these sets or none at all in your project submission.
If you are unsure what queries to generate (for e.g., what kind of query will require the use of Window Functions), we strongly recommend using questions 
from the question set.
****************************************************************************************************************************************************************

Question 1
We want to understand more about the movies that families are watching. The following categories are considered family movies: Animation, Children, Classics, Comedy, Family and Music.

Create a query that lists each movie, the film category it is classified in, and the number of times it has been rented out.

Check Your Solution
For this query, you will need 5 tables: Category, Film_Category, Inventory, Rental and Film. Your solution should have three columns: Film title, Category name and Count of Rentals.

The following table header provides a preview of what the resulting table should look like if you order by category name followed by the film title.

HINT: One way to solve this is to create a count of movies using aggregations, subqueries and Window functions.




Question 2
Now we need to know how the length of rental duration of these family-friendly movies compares to the duration that all movies are rented for. Can you provide a table with the movie titles and divide them into 4 levels (first_quarter, second_quarter, third_quarter, and final_quarter) based on the quartiles (25%, 50%, 75%) of the rental duration for movies across all categories? Make sure to also indicate the category that these family-friendly movies fall into.

Check Your Solution
The data are not very spread out to create a very fun looking solution, but you should see something like the following if you correctly split your data. You should only need the category, film_category, and film tables to answer this and the next questions. 

HINT: One way to solve it requires the use of percentiles, Window functions, subqueries or temporary tables.




Question 3
Finally, provide a table with the family-friendly film category, each of the quartiles, and the corresponding count of movies within each combination of film category for each corresponding rental duration category. The resulting table should have three columns:

Category
Rental length category
Count
Check Your Solution
The following table header provides a preview of what your table should look like. The Count column should be sorted first by Category and then by Rental Duration category.

HINT: One way to solve this question requires the use of Percentiles, Window functions and Case statements.

*****************************************************************************************************************************
######Question Set 2#######
The questions in this question set use the more advanced techniques of the course. These are meant to help you practice 
some of these more advanced techniques. Again, you have the choice to use any of these questions or use your own. Remember,
you need only to submit queries that meet the criteria as specified in the Rubric.
*****************************************************************************************************************************

Question 1:
We want to find out how the two stores compare in their count of rental orders during every month for all the years we have data for. Write a query that returns the store ID for the store, the year and month and the number of rental orders each store has fulfilled for that month. Your table should include a column for each of the following: year, month, store ID and count of rental orders fulfilled during that month.

Check Your Solution
The following table header provides a preview of what your table should look like. The count of rental orders is sorted in descending order.

HINT: One way to solve this query is the use of aggregations.




Question 2
We would like to know who were our top 10 paying customers, how many payments they made on a monthly basis during 2007, and what was the amount of the monthly payments. Can you write a query to capture the customer name, month and year of payment, and total payment amount for each month by these top 10 paying customers?

Check your Solution:
The following table header provides a preview of what your table should look like. The results are sorted first by customer name and then for each month. As you can see, total amounts per month are listed for each customer.

HINT: One way to solve is to use a subquery, limit within the subquery, and use concatenation to generate the customer name.


Question 3
Finally, for each of these top 10 paying customers, I would like to find out the difference across their monthly payments during 2007. Please go ahead and write a query to compare the payment amounts in each successive month. Repeat this for each of these 10 paying customers. Also, it will be tremendously helpful if you can identify the customer name who paid the most difference in terms of payments.



