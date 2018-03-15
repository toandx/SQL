# SQL 4
show databases;
use classicmodels;
show tables;

# Cau 1 
select * from customers where city in ('Nantes','Lyon');

# Cau 2
select * from orders where shippedDate between '2003/01/10' and '2003/03/10';

#Cau 3
select * from orders where shippedDate>='2003/01/10' and shippedDate<='2003/03/10';

#Cau 4
select * from products where productLine like '%cars%';

#Cau 5
select * from products order by quantityInStock DESC limit 10;

#Cau 6
select *, (quantityinstock*buyPrice) as Money from products;
