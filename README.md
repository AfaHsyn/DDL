# DDL

drop table students
create table students (
student_id number primary key,
first_name varchar2(50) ,
last_name varchar2(50),
age number)

alter table students
add  address varchar(100)

alter table students 
add  grade number


#DML

insert into students (student_id,first_name,last_name,age,address,grade) 
values (1,'Ali','Aliyev',19,'Baku',87); commit 

insert into students (student_id,first_name,last_name,age,address,grade) 
values (2,'Nigar','Hesenli',18,'Baku',76); commit 

insert into students (student_id,first_name,last_name,age,address,grade) 
values (3,'Leyla','Agayeva',20,'Sumgayit',56); commit 

update students 
set first_name='Azad'
where student_id=1


delete students 
where first_name='Azad'

#Select statements


select employee_id,max(salary)
from employees 
where salary > 600 and department_id=50
group by employee_id
order by employee_id desc
fetch first 10 rows only
