# Hospital_Management
Desktop application for hospital management 

# TOTAL MODULES

## ADMIN MODULE
	
- 1. Login
- 2. Manage Employees
  -	Add Employee
  -	Update Employee
  -	Remove Employee
  -	Show Employee
- 3. Manage Doctors
  -	Add Doctor
  -	Update Doctor
  -	Remove Doctor
  -	Show Doctor
- 4. Manage Receptionist
  -	Add Receptionist
  -	Update Receptionist
  -	Remove Receptionist
  -	Show Receptionist
- 5. View Patients 

## RECEPTIONIST MODULE
  1.	Login
  2.	Add Patient 
  3.	Update Patient
  4.	Remove Patient
  5.	Show Patient
  6.	Verify OTP

## DOCTOR MODULE
  1.	Login
  2.	View Appointments

_______________________________________________________________________________________________________________________________________________________

# FIRST OF ALL WE NEED TO DESIGN TABLES WHICH IS USED IN OUR PROJECT
  1.	EMPLOYEES
  2.	USERS
  3.	PATIENT
  4.	DOCTORS

## STRUCTURE OF TABLE EMPLOYEES

- Column Name 	 Data Type	                Description
- EMPID	         Varchar2(20)	              Contains EMPID of employees
- EMPNAME	       Varchar2(30)	              Contains Name of employees
- ROLE	         Varchar2(30)	              Contains type of employees
- SAL	           Number(8,2)	              Contains salary of employees

## STRUCTURE OF TABLE USERS

- Column Name	Data Type	Description	Constraint
- USERID	Varchar2(20)	Contains USERID of user	Primary Key
- USERNAME	Varchar2(30)	Contains username of user	Not Null
- EMPID	Varchar2(30)	Contains empid of user	Foreign Key
- PASSWORD	Varchar2(30)	Contains password of user	Not Null
- USERTYPE	Varchar2(20)	Contains usertype of user	Not Null


## STRUCTURE OF TABLE PATIENT

- Column Name	Data Type	Description	Constraint
- P_ID	Varchar2(20)	Contains unique id of patient	Primary Key
- F_NAME	Varchar2(30)	Contains first name of patient	Not Null
- S_NAME	Varchar2(30)	Contains last name of patient	Not Null
- AGE	Varchar2(30)	Contains age of patient	Not Null
- OPD	Varchar2(20)	Contains OPD	Not Null
- GENDER	Varchar2(10)	Contains gender of patient	Not Null
- M_STATUS	Varchar2(20)	Contains marital status of patient	Not Null
- P_DATE	Date	Contains date of appointment	Not Null
- ADDRESS	Varchar2(100)	Contains address of patient	Not Null
- CITY	Varchar2(25)	Contains city of patient	Not Null
- PHONE_NO	Varchar2(13)	Contains mobile number of patient	Not Null
- DOCTOR_ID	Varchar2(10)	Contains Doctor_Id	Foreign Key
- OTP	Number(7)	Contains OTP which	Not Null

## STRUCTURE OF TABLE DOCTORS
- Column Name	Data Type	Description	Constraint
- USERID	Varchar2(20)	Contains userid of doctor	Foreign Key
- DOCTORID	Varchar2(20)	Contains doctor_id of doctor	Primary Key
- QUALIFICATION	Varchar2(30)	Contains qualification of doctor	Not Null
- SPECIALIST	Varchar2(50)	Contains specialization of doctor	Not Null



