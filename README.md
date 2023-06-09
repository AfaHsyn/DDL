# DDL

drop table students
create table students (
student_id number primary key,
first_name varchar2(50) ,
last_name varchar2(50),
age number)

alter table students
add  address varchar(100)
