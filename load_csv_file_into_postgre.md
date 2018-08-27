Background: I'm working with very large datasets, and find it hard to join large tables using pandas. So I wanted to load cleaned data into postgres and do the joining there. Things look positive so far.

How I did it:

Solution 1 -- using sqlalchemy and pandas built-in function.

1. I already had psycopg2 and sqlalchemy installed.

2. Made sure the file going into postgres has column names.

3. Created an sqlalchemy engine.

4. Used pandas.DataFrame.to_sql() and load the file into database directly.

5. All done!


Notes for future exploration:

Another option is to use psycopg2: create table first and load data into database with sql commands.

But so far pandas' built-in function is pretty straightforward and meets my need. However, not sure if there is a more efficient way to do this. 
