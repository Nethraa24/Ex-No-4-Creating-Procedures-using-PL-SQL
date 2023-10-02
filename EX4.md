# Ex. No: 4 Creating Procedures using PL/SQL

### AIM: To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:

Create table :

 create table emp2(Emp_id NUMBER,Ename varchar (100) , Dept varchar(20) , Salary NUMBER);

Create Procedure :

create or replace procedure insert_emp_data as



begin



insert into emp2(Emp_id,Ename,Dept,Salary)


values(1,'Nethraa', 'HR' , 50000);

insert into emp2(Emp_id,Ename,Dept,Salary)

values (2,'Hari' , 'IT',50000);

insert into emp2(Emp_id,Ename,Dept,Salary)

values (3,'Kothai' , 'Finance',50000);

insert into emp2(Emp_id,Ename,Dept,Salary)

values (4,'Keerthi' , 'IT',50000);

commit;

end;

/

Call Procedure :

begin


insert_emp_data;


end;


/




select *from emp2;




### Output:
![image](https://github.com/Nethraa24/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/121215786/84857ac4-a640-4c74-bd8d-1d73ac16390e)

### Result:
Thus a procedure is created using PL/SQL.
