# CohortsAnalysisPythonSQL

Consider 2 tables
Table1 of orders with columns:
1. order_id (integer, unique, not null, primary key)
2. user_id (integer, not null, foreign key)
3. order_amount (float, not null)
4. order_date (timestamp, not null)

Table2 of users with columns:
1. user_id (integer, unique, not null, primary key)
2. first_name (character, not null)
3. last_name (character, not null)
4. referral_code (character, unique, not null)
5. referred_by_code (character)
6. date_joined (timestamp, not null)


The order amount is the amount of money spent on the order. Write a query
to perform a (simple) cohort analysis. Define a "cohort" as a group of people who signed up for
our service in a particular month and year. Compute the average amount spent per individual in
the cohort in their first year as customers (one year from when they joined). Analyze just the
cohorts that joined in the year 2014. The output table should have two columns: "Cohort Month"
and "Average Cohort Spending" and 12 rows, one for each month in the year 2014. 
