# INTRODUCTION
 Hi,I'm sammie,I have been learning SQL for a while and this is my 1st project,This Project is to help me Optimize my Knowledge of SQL. 
# PROBLEM STATEMENT

# SKILLS DEMONSTRATED
I used PostgreSQL,putting to use Clauses like  WHERE,LIMIT,GROUP BY,ORDER BY,JOINS,wINDOWS FUNCTION 
# DATA SOURCING
 For this project I created 3 tables tagged Sales Table,Menu Table,Members Table
 I created a Schema Named Assessment,You can Run the below Script to Create this tables too 
 
Table 1- Sales Table
create table assessment.sales_table 
(
		customer_id varchar(30),
		order_date date,
		product_id int
)

insert into assessment.sales_table
values ('A1', '2021-01-01', 1),
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
create table assessment.menu_table 
(
		product_id int,
		product_name varchar(50),
		price int
)


insert into assessment.menu_table
VALUES (1, 'Salad', 10),
	   (2, 'Coke', 15),
	   (3, 'Rice', 12)


Table 3 - Members Table
create table assessment.members_table 
(
		customer_id varchar(30),
		join_date date
)

insert into assessment.members_table
values 		('A1', '2021-01-07'),
		('B1', '2021-01-09')
			
# DATA ANALYSIS AND VISUALISATION
# CONCLUSION
