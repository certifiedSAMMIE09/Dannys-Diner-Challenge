# INTRODUCTION
- Hi, I'm Sammie, I have been learning SQL for a while and I stumbled on Danny's Diner 8 weeks SQL challenge, SO I decided to work on it. This project enabled me put to work all that has been learnt overtime. 
# PROBLEM STATEMENT
Danny wants to use the data to answer a few simple questions about his customers, especially about their visiting patterns, how much money they’ve spent and also which menu items are their favourite. Having this deeper connection with his customers will help him deliver a better and more personalised experience for his loyal customers.

He plans on using these insights to help him decide whether he should expand the existing customer loyalty program - additionally he needs help to generate some basic datasets so his team can easily inspect the data without needing to use SQL.

Danny has provided you with a sample of his overall customer data due to privacy issues - but he hopes that these examples are enough for you to write fully functioning SQL queries to help him answer his questions!

Danny has shared with you 3 key datasets for this case study:
- Sales
- Menu
- Members 

# SKILLS DEMONSTRATED
- I used PostgreSQL,putting to use clauses like WHERE, LIMIT, GROUP BY, ORDER BY, JOINS, WINDOWS FUNCTION 

# DATA SOURCING
-  For this project I created 3 tables tagged Sales Table,Menu Table,Members Table
 I created a Schema named dannys_diner, You can run the below Script to create these tables too:
 CREATE SCHEMA dannys_diner;
 SET search_path = dannys_diner;

 
Table 1- Sales Table
CREATE TABLE sales (
  "customer_id" VARCHAR(1),
  "order_date" DATE,
  "product_id" INTEGER
);

insert into dannys_diner.sales_table
values     ('A1', '2021-01-01', 1),
	   ('A1', '2021-01-01', 2),
	   ('A1', '2021-01-07', 2),
	   ('A1', '2021-01-10', 3),
	   ('A1', '2021-01-11', 3),
	   ('A1', '2021-01-11', 3),
	   ('B1', '2021-01-01', 2),
	   ('B1', '2021-01-02', 2),
	   ('B1', '2021-01-04', 1),
	   ('B1', '2021-01-11', 1),
	   ('B1', '2021-01-16', 3),
	   ('B1', '2021-02-01', 3),
	   ('C1', '2021-01-01', 3),
	   ('C1', '2021-01-01', 3),
	   ('C1', '2021-01-07', 3);
	   



Table 2 -Menu Table
create table dannys_diner.menu_table 
(
		product_id int,
		product_name varchar(50),
		price int
)


INSERT INTO menu
("product_id", "product_name", "price")
VALUES
  ('1', 'sushi', '10'),
  ('2', 'curry', '15'),
  ('3', 'ramen', '12');


Table 3 - Members Table
create table dannys_diner.members_table 
(
		customer_id varchar(30),
		join_date date
)

insert into dannys_diner.members_table
values 		('A1', '2021-01-07'),
		('B1', '2021-01-09')
			
# DATA ANALYSIS AND VISUALISATION
# CONCLUSION
