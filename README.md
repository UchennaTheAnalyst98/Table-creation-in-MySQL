#     DATABASE AND TABLE CREATION;

DROP DATABASE IF EXISTS deff;

CREATE DATABASE IF NOT EXISTS deff;

USE deff;

CREATE TABLE employees (
	  employee_id INT AUTO_INCREMENT,
    first_name VARCHAR(30) NOT NULL,
    last_name VARCHAR(30) NOT NULL,
    gender CHAR(10),
    PRIMARY KEY (employee_id)
);

SELECT *
FROM employees;


# ADDING DETAILS OF THE VARIOUS EMPLOYEES INTO THE TABLE;

INSERT INTO employees (first_name, last_name, gender)
VALUES	('Uchenna', 'Joseph', 'male'),
		    ('Gideon', 'Jordan', 'male'),
        ('Sarah', 'Kefas', 'female'),
        ('Onyiyechi', 'Emmanuel', 'female');
        
SELECT *
FROM employees;
