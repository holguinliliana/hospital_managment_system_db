# Hospital Management System Database
## Description
### Overview
> This database is ment to hold and organize patient, doctor, nurse, and room information.
### Patient
> The "PATIENT" table holds the basic questionare information a patienet would fill out when being admitted into the hospital.
> The "PATIENT" table also holds one-to-one relation and a one-to-many relation to "emergencyContact", "INSURANCE", "ROOMS", "TREATMENT", and "PAYMENT".
### Doctor
> The "DOCTOR" table holds the doctors' basic information, similar to the "PATIENT" table, with the exeption of the admission details, rather replacing it with their certification, position, department, and salary.
### Nurse
> The "NURSE" table holds the nurses' basic information, similar to the "DOCTOR" table, with the exeption of their department.
> The "NURSE" table also holds a one-to-one relation with the "ROOM" table.
## Author
## Liliana Holguin
> email: hollil@nmsu.edu <br>
> github: https://github.com/holguinliliana
## Getting Started
### Dependencies
> The only true dependency that this database requires is the ability to hold the sqlite application.
### Executing the Database
> Realistically, the hospital staff would temporarily store their information somewhere else, before having it implamented into the database.
> However, when transfering the data, mainly new data, they would just have to write the "INSERT INTO table VALUES (...);" command, inserting the data accordingly.
### Step-by-Step Example
1. .open hospital_management.db
2. INSERT INTO PATIENT VALUES ('3373244', 'Sade Almond ', '1995-24-04', '193751721', '1337  Cooks Mine Road', '507-642-5979', 'F', 'single', 'Dr. Radomira', 'Breast Cancer', 'Cancer Treatment', '2021-01-07', '2021-01-12');
   * With the order and data types being:
   >patient_id (int),patient_name (char(50)),patient_dob (DATE),patient_SS_no (int),p_address (text),p_phone_no (char(50)),patient_sex (char),patient_marital_status (char(50)),primary_care_provider (text),prior_med_condition (text),reason_for_admission (text),admission_dt (DATE),discharge_dt(DATE)
   * In which the genaric synatx being:
   >INSERT INTO PATIENT(patient_id,patient_name,patient_dob,patient_SS_no,p_address,p_phone_no,patient_sex,patient_marital_status,primary_care_provider,prior_med_condition,reason_for_admission,admission_dt,discharge_dt)VALUES (data);
 3. Repeated until all data has been inserted.
 ## Output
 > Although there is not a concrete output seen in java programs, it would be appropitate to say that the output of the database is a database holding, primarily, tables with patient, doctor, nurse, and room information.
 
