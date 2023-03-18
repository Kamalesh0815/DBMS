# DBMS

USE store ;
![image](https://user-images.githubusercontent.com/118426240/226111130-33f112bd-0bf3-456f-ba4b-9d1a0c49e8ff.png)

SHOW tables;
![image](https://user-images.githubusercontent.com/118426240/226111186-51f96d72-8c0f-484a-a8dc-71601f85cb27.png)

SELECT * FROM customers;
![image](https://user-images.githubusercontent.com/118426240/226111212-c0d26945-5c01-4d14-9fd7-a7263d0ea87d.png)

SELECT * FROM  customers order by  first_name DESC;
![image](https://user-images.githubusercontent.com/118426240/226111234-7c99344d-811d-4a28-a757-51ac27d30da2.png)

SELECT 1,2;
![image](https://user-images.githubusercontent.com/118426240/226111253-774025da-45f2-4a58-8ddf-c3a51cb5ba67.png)

SELECT 1+2;
![image](https://user-images.githubusercontent.com/118426240/226111264-702d15db-d855-4d29-8e07-e6bebafa026a.png)

SELECT 100-50/2 AS Answer;
![image](https://user-images.githubusercontent.com/118426240/226111436-29b1fced-9368-4f36-9e52-3797ed493847.png)

SELECT 100-50/2 AS 'answer value';
![image](https://user-images.githubusercontent.com/118426240/226111445-41ded271-36c7-42dc-ba20-24e6da4836f1.png)

SELECT 171*214+625 AS answer;
![image](https://user-images.githubusercontent.com/118426240/226111402-cbfc6a23-51d5-4cb4-8f77-55fa183bfb28.png)


SELECT first_name,last_name,points,points +10 FROM customers;
SELECT first_name,last_name,points  FROM customers;
![image](https://user-images.githubusercontent.com/118426240/226111338-27c32f9a-52e8-4832-8e68-c0204988f181.png)

SELECT first_name,last_name,points,points +10 AS 'new Points' FROM customers;
![image](https://user-images.githubusercontent.com/118426240/226111364-73dc9800-bbcc-4ff4-bf12-f340e387e1a5.png)

SELECT FIRST_NAME AS 'First Name' , LAST_NAME AS 'Last Name' FROM employees;
![image](https://user-images.githubusercontent.com/118426240/226111500-fe029750-8880-4fe9-9114-ada2c13f29a8.png)

SELECT FIRST_NAME,LAST_NAME,SALARY,SALARY * 15/100 AS  'PF'	 FROM employees;
![image](https://user-images.githubusercontent.com/118426240/226111532-533cf5d9-91fb-4768-a6e0-9d8236b04967.png)

SELECT DISTINCT DEPARTMENT_ID FROM employees;
![image](https://user-images.githubusercontent.com/118426240/226111558-7de64a9d-5ebc-4fb9-a060-71dcb1623a68.png)

SELECT name,unit_price,1.1 * unit_price AS 'new price' FROM products;
![image](https://user-images.githubusercontent.com/118426240/226111594-df223cd9-7a52-432e-9426-8b6460e41e50.png)

SELECT * FROM customers WHERE state = 'FL';
![image](https://user-images.githubusercontent.com/118426240/226111608-5792bc3a-65bb-4e8f-8d5d-23c42241e273.png)

SELECT * FROM customers WHERE points > 3000;
![image](https://user-images.githubusercontent.com/118426240/226111618-32a8acff-e64d-4ce6-85a6-fdaf163da04d.png)

SELECT * FROM customers WHERE birth_date >= '1990-01-01';
![image](https://user-images.githubusercontent.com/118426240/226111637-878d1717-3453-4d11-ba8c-1242aa670fac.png)

SELECT * FROM customers WHERE state != 'FL';
![image](https://user-images.githubusercontent.com/118426240/226111653-6fdbadfb-7be5-4165-a788-5d6df4038351.png)

SELECT * FROM customers WHERE NOT ( state = 'FL');
![image](https://user-images.githubusercontent.com/118426240/226111683-17a5b7a3-dcbe-4632-b4f1-169ad79d404d.png)

SELECT * FROM customers WHERE points > 3000 AND birth_date >= '1990-01-01';
![image](https://user-images.githubusercontent.com/118426240/226111722-bea0fc33-dcd1-435b-b161-49566df84c98.png)

SELECT * FROM customers WHERE points > 3000 OR birth_date >= '1990-01-01';
![image](https://user-images.githubusercontent.com/118426240/226111744-a3b33f40-a5a7-471e-bf83-ef88c0c4e6e1.png)

SELECT * FROM customers WHERE birth_date > '1889-01-01' OR (points > '1000' AND state = 'VA');
![image](https://user-images.githubusercontent.com/118426240/226111771-ba1a8128-222e-4c66-8ae2-4969e7fd5142.png)

SELECT * FROM customers WHERE (birth_date > '1989-01-01' AND points > '1000') OR state = 'VA';
![image](https://user-images.githubusercontent.com/118426240/226111785-72aef96d-a2af-43d9-8c6e-47f900f48ebc.png)

SELECT * FROM customers WHERE state = 'VA' OR state= 'FL'  OR state = 'GA';
![image](https://user-images.githubusercontent.com/118426240/226111808-589ea471-e121-4265-b4c1-c59bd35e7c39.png)

SELECT * FROM employees order by first_name DESC; 
![image](https://user-images.githubusercontent.com/118426240/226111889-2ec69003-16c1-41cb-b530-5baa74dd90ac.png)

SELECT EMPLOYEE_ID,FIRST_NAME, LAST_NAME,SALARY FROM employees;
![image](https://user-images.githubusercontent.com/118426240/226111898-2e9ad1a5-2100-43ae-a0e2-f98a8b1e68f7.png)

SELECT first_name,last_name,hire_date
FROM employees
WHERE hire_date BETWEEN '1987-01-01' AND '1987-12-30';
![image](https://user-images.githubusercontent.com/118426240/226111918-b27bd63f-7f85-482d-977d-3fe11be3d0aa.png)

SELECT first_name,last_name,salary 
FROM employees
WHERE salary NOT BETWEEN 10000 AND 15000;
![image](https://user-images.githubusercontent.com/118426240/226111929-811cff2b-c1d6-4d72-bac1-7c4b9672bc73.png)

SELECT first_name,last_name,department_id 
FROM employees
WHERE department_id = 30 OR department_id = 100 
ORDER BY department_id ASC;
![image](https://user-images.githubusercontent.com/118426240/226111963-7fa51d30-b754-4c34-865b-345df6b0c98d.png)

SELECT first_name,last_name,salary 
FROM employees
WHERE (salary NOT BETWEEN 10000 AND 15000) AND (department_id = 30 OR department_id = 100);
![image](https://user-images.githubusercontent.com/118426240/226111994-18e2af28-2fe4-4301-b2eb-638e1bd90b53.png)

SELECT *
FROM employees
WHERE last_name IN ('BLAKE', 'SCOTT', 'KING','FORD');
![image](https://user-images.githubusercontent.com/118426240/226112010-9726ff39-7fe7-4d9c-8439-d8905e61a5c9.png)

SELECT * FROM products WHERE quantity_in_stock IN (49,38,72);
![image](https://user-images.githubusercontent.com/118426240/226112095-e031b8c8-fc1a-48d7-a174-9719edf29eef.png)

SELECT * FROM products WHERE quantity_in_stock NOT IN (72);
![image](https://user-images.githubusercontent.com/118426240/226112116-fd7ed465-9c82-4813-a49f-e0a1dcbf2c45.png)

 select employee_id,first_name,last_name,e.department_id,department_name  from employees as e inner join departments   as d
 on e.department_id = d.department_id where department_name = "IT" ;
![image](https://user-images.githubusercontent.com/118426240/226112160-0c4999a6-a99e-4f45-8c68-64d3486d7b6d.png)

select * from todos order  by duedate;
![image](https://user-images.githubusercontent.com/118426240/226112204-fa56d425-2ed9-43cb-89dd-16134742ecd2.png)

select * from todos where task like '%dry%';
![image](https://user-images.githubusercontent.com/118426240/226112218-e63dafff-795b-449e-8f0f-6efd36685ba8.png)

select * from todos where dueDate > '2023-02-18' order by dueDate;
![image](https://user-images.githubusercontent.com/118426240/226112235-76bf1ece-8ab9-455c-922e-a3e3a6b6f80a.png)

select * from todos where dueDate between '2023-02-20' and '2023-02-24' order by dueDate;
![image](https://user-images.githubusercontent.com/118426240/226112247-996db120-c841-467f-9993-f7d9bca86f75.png)

SELECT * FROM todos WHERE dueDate IN ('2023-02-17',
'2023-02-24',
'2023-03-03',
'2023-02-17',
'2023-02-24',
'2023-03-03',
'2023-02-17',
'2023-02-24',
'2023-03-03',
'2023-02-17',
'2023-02-24',
'2023-03-03',
'2023-02-17',
'2023-02-24',
'2023-03-03',
'2023-02-17',
'2023-02-24',
'2023-03-03',
'2023-02-17',
'2023-02-24',
'2023-03-03');
![image](https://user-images.githubusercontent.com/118426240/226112300-61264ac2-b316-42b9-bbb5-abfb84012489.png)

select * from todos where id in ('10');
![image](https://user-images.githubusercontent.com/118426240/226112319-1f393853-c18d-40cf-83c2-3df474ae2b6d.png)

select * from todos where dueDate = '2023-02-17' or dueDate = '2023-02-24' or dueDate = '2023-03-03';
![image](https://user-images.githubusercontent.com/118426240/226112334-8972a527-ab96-4c2c-bd1c-bf307a268d65.png)

SELECT * FROM todos ORDER BY dueDate,task;
![image](https://user-images.githubusercontent.com/118426240/226112356-5aceb2b7-1466-4475-9141-6fbd94467fbb.png)

SELECT * FROM todos WHERE task REGEXP '^Buy' AND task REGEXP 'shoes$';
![image](https://user-images.githubusercontent.com/118426240/226112374-ac5d9a2f-c4e2-457f-8f2a-8440c63d9b4e.png)

SELECT COUNT(id) FROM todos;
![image](https://user-images.githubusercontent.com/118426240/226112434-df7792d6-d57b-447b-9ba3-9ae2e1f8e808.png)

SELECT MAX(dueDate) FROM todos; 
![image](https://user-images.githubusercontent.com/118426240/226112503-3d141e5c-594f-4c7a-8b9f-a396c02b675a.png)

SELECT DATEDIFF(dueDate,"2023-02-16") AS "Left Days"
FROM todos
WHERE task = 'Buy groceries' ;
![image](https://user-images.githubusercontent.com/118426240/226112502-5d730322-c855-4596-9c2e-bf31f47e23bb.png)

-- Write a query to get the total salaries payable to employees.
SELECT SUM(salary) AS "Total Salary"
FROM employees;
![image](https://user-images.githubusercontent.com/118426240/226112510-0b2b5fcb-0492-4fd1-bdf7-e95ae948614b.png)

-- Write a query to get the maximum and minimum salary from employees table.
SELECT MAX(salary) AS "Maximum Salary",MIN(salary) AS "Minimum Salary"
FROM employees;
![image](https://user-images.githubusercontent.com/118426240/226112522-43223a79-96e2-4537-a682-469b488eec93.png)

-- Write a query to get the average salary and number of employees in the employees table.
SELECT AVG(salary) AS "Average Salary",COUNT(salary) AS "Number of employees"
FROM employees;
![image](https://user-images.githubusercontent.com/118426240/226112532-b1620497-c523-4160-9505-66c511c0f7b9.png)

-- Write a query to get the number of employees working with the company.
SELECT COUNT(*) AS "Number of employees"
FROM employees;
![image](https://user-images.githubusercontent.com/118426240/226112551-cf7ca635-fc79-49a8-a215-9b9c91f34b7c.png)

-- Write a query to get the number of distinct jobs available in the employees table.
SELECT COUNT(DISTINCT job_id) 
FROM employees;
![image](https://user-images.githubusercontent.com/118426240/226112578-ebaac175-b6ed-4dd9-ac57-0d013ad2f5dc.png)

-- Write a query get all first name from employees table in upper case.
SELECT UCASE(first_name) AS "First Name"
FROM employees;

CREATE TABLE todos_gitHub 
(id INT PRIMARY KEY AUTO_INCREMENT,
task VARCHAR(255),
dueDate DATE,
isEditing TINYINT);
describe todos_gitHub ;
![image](https://user-images.githubusercontent.com/118426240/226112674-2cf6b307-a4ac-449d-b662-f622c95f08b7.png)

INSERT INTO todos_gitHub (task, dueDate, isEditing) VALUES 
('Finish writing report', '2023-03-05', 0),
('Buy groceries', '2023-02-20', 0),
('Book dentist appointment', '2023-02-21', 0),
('Prepare for presentation', '2023-03-02', 0),
('Clean the house', '2023-02-24', 0),
('Go for a run', '2023-02-17', 0),
('Read a book', '2023-02-22', 0),
('Meet with client', '2023-03-01', 0),
('Pay rent', '2023-02-28', 0),
('Plan vacation', '2023-03-10', 0),
('Attend yoga class', '2023-02-18', 0),
('Finish coding project', '2023-03-07', 0),
('Visit grandparents', '2023-02-27', 0),
('Buy new shoes', '2023-02-25', 0),
('Do laundry', '2023-02-19', 0),
('Take dog for a walk', '2023-02-21', 0),
('Send out invoices', '2023-03-04', 0),
('Get a haircut', '2023-02-23', 0),
('Meet with colleagues', '2023-02-28', 0),
('Create marketing plan', '2023-03-03', 0),
('Practice guitar', '2023-02-20', 0),
('File taxes', '2023-03-15', 0),
('Buy birthday gift', '2023-03-08', 0),
('Go to the gym', '2023-02-19', 0),
('Make doctor appointment', '2023-02-23', 0),
('Finish online course', '2023-03-06', 0),
('Clean out closet', '2023-02-24', 0),
('Meet with mentor', '2023-03-01', 0),
('Pay credit card bill', '2023-03-02', 0),
('Go on a hike', '2023-02-18', 0),
('Start new project', '2023-03-05', 0),
('Buy plane tickets', '2023-03-10', 0),
('Meet with friend', '2023-03-08', 0),
('Get oil change', '2023-02-23', 0),
('Organize desk', '2023-02-21', 0),
('Submit job application', '2023-03-07', 0),
('Buy new phone', '2023-02-25', 0),
('Go to dentist', '2023-03-12', 0),
('Clean out fridge', '2023-02-24', 0),
('Finish book', '2023-02-22', 0),
('Attend networking event', '2023-03-04', 0),
('Take online course', '2023-02-20', 0),
('Plan dinner party', '2023-03-10', 0),
('Meet with business partner', '2023-03-01', 0),
('Submit proposal', '2023-03-05', 0);
![image](https://user-images.githubusercontent.com/118426240/226112720-c7b3e8ae-b506-4bb3-9d43-ea041b5545d1.png)

ALTER TABLE todos_gitHub
ADD whatsapp_No_gitHub int;
describe todos_gitHub ;
![image](https://user-images.githubusercontent.com/118426240/226112793-b5ae5751-e991-4929-9d7b-8678254ccf6d.png)

ALTER TABLE user
ADD test int ;
![image](https://user-images.githubusercontent.com/118426240/226112882-c587cc02-3827-4356-8cf0-ed3361fa8387.png)

alter table user rename column test to new;
![image](https://user-images.githubusercontent.com/118426240/226112925-db8b0f57-e78b-4f55-9405-b5ab8dc38f9e.png)


INSERT INTO user (username,password,dob,phone,email,first_name,last_name,new)
VALUES ('test1', 'test2', '2022-02-02','test4','test5','test6','test7','0987654321');
<img width="521" alt="image" src="https://user-images.githubusercontent.com/118426240/226113016-3cfe5469-9f12-42ad-90a0-425ee4e74e29.png">

UPDATE user
SET username='Alfred Schmidt', last_name='Frankfurt'
WHERE new=987654321;
![image](https://user-images.githubusercontent.com/118426240/226113058-b6d2bd0c-5e45-43fe-a27a-0be610625c37.png)

ALTER TABLE countries
ADD REGION_ID  decimal(10,0);
![image](https://user-images.githubusercontent.com/118426240/226113101-ee9a2f2b-fc46-49ef-8be1-ef58ec652eb2.png)

ALTER TABLE countries
DROP COLUMN REGION_ID;
![image](https://user-images.githubusercontent.com/118426240/226113166-c6c0433b-5916-4119-a09f-6af987a2e8eb.png)

INSERT INTO countries (COUNTRY_ID,COUNTRY_NAME,REGION_NAME)
VALUES ('21','India','33333');
![image](https://user-images.githubusercontent.com/118426240/226113203-1b9a47b3-55ad-4f61-91c6-31a86265c714.png)

INSERT INTO countries (COUNTRY_ID,COUNTRY_NAME)
VALUES ('25','AUS');
![image](https://user-images.githubusercontent.com/118426240/226113211-97452760-b83e-4bca-b54a-bf2430fb0b9f.png)

UPDATE countries
SET COUNTRY_ID = null;
![image](https://user-images.githubusercontent.com/118426240/226113246-ff099f39-865d-4a53-a70a-423004cfc074.png)

SELECT  d.department_id, d.department_name, first_name, last_name
FROM employees AS e inner join departments AS d
ON e.department_id = d.department_id;
![image](https://user-images.githubusercontent.com/118426240/226113270-39f355ec-99f0-403a-93a5-12e00d686d51.png)

SELECT j.job_title, e.first_name, min_salary,e.job_id,j.job_id,e.salary
FROM employees AS e inner join jobs AS j
ON e.job_id = j.job_id;
![image](https://user-images.githubusercontent.com/118426240/226113286-f6dbea83-405c-46ba-97b9-919436f64bc0.png)

SELECT jh.employee_id, j.job_title, jh.end_date-jh.start_date Days, jh.department_id
FROM  jobs AS j inner join  job_history AS jh
ON j.job_id = jh.job_id
WHERE department_id=90;
![image](https://user-images.githubusercontent.com/118426240/226113304-fd7d3639-489d-414e-b53f-831e5f6ddfcc.png)

SELECT d.department_name, e.first_name, l.city
FROM departments AS d  INNER JOIN employees AS e  inner join locations AS l
ON d.manager_id = e.employee_id; 
![image](https://user-images.githubusercontent.com/118426240/226113339-7a72d6c3-58c9-4b64-ab3c-259616146ca0.png)








