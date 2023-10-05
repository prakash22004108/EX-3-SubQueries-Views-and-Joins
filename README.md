# EX-3-SubQueries-Views-and-Joins
# EX-3-SubQueries-Views-and-Joins


## Create employee Table
```sql
CREATE TABLE EMP (EMPNO NUMBER(4) PRIMARY KEY,ENAME VARCHAR2(10),JOB VARCHAR2(9),MGR NUMBER(4),HIREDATE DATE,SAL NUMBER(7,2),COMM NUMBER(7,2),DEPTNO NUMBER(2));
```
## Insert the values
INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO)
VALUES (7369, 'SMITH', 'CLERK', 7902, '17-DEC-80', 800, NULL, 20);
INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO)
VALUES (7499, 'ALLEN', 'SALESMAN', 7698, '20-FEB-81', 1600, 300, 30);
INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO)
VALUES (7521, 'WARD', 'SALESMAN', 7698, '22-FEB-81', 1250, 500, 30);
INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO)
VALUES (7566, 'JONES', 'MANAGER', 7839, '02-APR-81', 2975, NULL, 20);
INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO)
VALUES (7654, 'MARTIN', 'SALESMAN', 7698, '28-SEP-81', 1250, 1400, 30);
INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO)
VALUES (7934, 'MILLER', 'CLERK', 7782, TO_DATE('23-JAN-82', 'DD-MON-RR'), 1300, 10, 10);
```
## Create department table
```sql
CREATE TABLE DEPT (DEPTNO NUMBER(2) PRIMARY KEY,DNAME VARCHAR2(14),LOC VARCHAR2(13));
```
## Insert the values in the department table
```sql
INSERT INTO DEPT (DEPTNO, DNAME, LOC) VALUES (10, 'ACCOUNTING', 'NEW YORK');
INSERT INTO DEPT (DEPTNO, DNAME, LOC) VALUES (20, 'RESEARCH', 'DALLAS');
INSERT INTO DEPT (DEPTNO, DNAME, LOC) VALUES (30, 'SALES', 'CHICAGO');
INSERT INTO DEPT (DEPTNO, DNAME, LOC) VALUES (40, 'OPERATIONS', 'BOSTON');
```
### Q1) List the name of the employees whose salary is greater than that of employee with empno 7566.


### QUERY:
![image](https://github.com/DhanushPalani/EX-3-SubQueries-Views-and-Joins/assets/121594640/1848b392-372d-4111-af2d-25daf5458864)


### OUTPUT:
![image](https://github.com/DhanushPalani/EX-3-SubQueries-Views-and-Joins/assets/121594640/ee7dd795-bf87-4dff-aca9-b80307477ddd)

### Q2) List the ename,job,sal of the employee who get minimum salary in the company.

### QUERY:
![image](https://github.com/DhanushPalani/EX-3-SubQueries-Views-and-Joins/assets/121594640/2c78d720-f077-4843-bbbd-cefb0e36afcf)


### OUTPUT:
![image](https://github.com/DhanushPalani/EX-3-SubQueries-Views-and-Joins/assets/121594640/0ca9e7dc-c9b6-45c6-b7a0-bf123d815295)

### Q3) List ename, job of the employees who work in deptno 10 and his/her job is any one of the job in the department ‘SALES’.

### QUERY:
![image](https://github.com/DhanushPalani/EX-3-SubQueries-Views-and-Joins/assets/121594640/ea1201a0-53bc-436b-b815-3889759afcff)


### OUTPUT:
![image](https://github.com/DhanushPalani/EX-3-SubQueries-Views-and-Joins/assets/121594640/7376ae95-bab6-4739-abd7-bdc5e8a727dd)


### Q4) Create a view empv5 (for the table emp) that contains empno, ename, job of the employees who work in dept 10.

### QUERY:
![image](https://github.com/DhanushPalani/EX-3-SubQueries-Views-and-Joins/assets/121594640/4c3e781f-8787-461d-b2ee-162f5222abd9)


### OUTPUT:
![image](https://github.com/DhanushPalani/EX-3-SubQueries-Views-and-Joins/assets/121594640/753d1db9-8955-4b97-b850-43622886968b)

### Q5) Create a view with column aliases empv30 that contains empno, ename, sal of the employees who work in dept 30. Also display the contents of the view.

### QUERY:

![image](https://github.com/DhanushPalani/EX-3-SubQueries-Views-and-Joins/assets/121594640/3551ed65-3cb5-4846-b817-48436b507530)

### OUTPUT:
![image](https://github.com/DhanushPalani/EX-3-SubQueries-Views-and-Joins/assets/121594640/026712b5-02b2-40d6-a757-cec5bc08890d)

### Q6) Update the view empv5 by increasing 10% salary of the employees who work as ‘CLERK’. Also confirm the modifications in emp table

### QUERY:
![image](https://github.com/DhanushPalani/EX-3-SubQueries-Views-and-Joins/assets/121594640/d83bbdcd-83a3-427e-bd2b-e799958b055d)


### OUTPUT:
![image](https://github.com/DhanushPalani/EX-3-SubQueries-Views-and-Joins/assets/121594640/6941b531-33ed-41dc-b6f4-9e8bcc0dd113)

## Create a Customer1 Table
INSERT INTO Salesman1 (salesman_id, name, city, commission) VALUES(5003, 'Lauson
### Q7) Write a SQL query to find the salesperson and customer who reside in the same city. Return Salesman, cust_name and city.

### QUERY:
![image](https://github.com/SivaChandranR07/EX-3-SubQueries-Views-and-Joins/assets/113497395/3b545832-cd20-4677-acc2-54a182519743)



### OUTPUT:
![image](https://github.com/SivaChandranR07/EX-3-SubQueries-Views-and-Joins/assets/113497395/124ad06c-99f3-4546-a47f-7d47d63814cc)



### OUTPUT:
![image](https://github.com/SivaChandranR07/EX-3-SubQueries-Views-and-Joins/assets/113497395/9cd2dd33-a619-4b80-b3c0-89cf9985d9cf)


### Q9) Perform Natural join on both tables

### QUERY:
![image](https://github.com/SivaChandranR07/EX-3-SubQueries-Views-and-Joins/assets/113497395/456bd1cd-d65d-4b4c-99fb-1169caf8e155)



### OUTPUT:
![image](https://github.com/SivaChandranR07/EX-3-SubQueries-Views-and-Joins/assets/113497395/488ccbba-0b6b-4b6a-b3e5-6af95242bd61)


### Q10) Perform Left and right join on both tables

### QUERY:
   ## Left Join
![image](https://github.com/SivaChandranR07/EX-3-SubQueries-Views-and-Joins/assets/113497395/54f15540-3169-4b76-9db1-704b4bf47476)


### OUTPUT:
   ## Left Join
![image](https://github.com/SivaChandranR07/EX-3-SubQueries-Views-and-Joins/assets/113497395/c9ed1e5d-d539-4663-82b9-fd4cff719b97)



   ## Right Join
![image](https://github.com/SivaChandranR07/EX-3-SubQueries-Views-and-Joins/assets/113497395/5a12564c-7f3e-40a1-ae0b-10e9816a5a33)
