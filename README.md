# 🚔 Crime Management System

## 📌 Project Overview

The Crime Management System is a database-driven project developed using Oracle SQL to digitally manage crime records, FIR registrations, criminal information, victim details, police stations, officers, and case files. The system helps law enforcement agencies maintain accurate records, reduce paperwork, improve data security, and efficiently track criminal activities.

---

## 🎯 Objective

The main objective of this project is to design and develop a centralized database system that helps police departments:

* Manage crime records efficiently
* Register and track FIRs
* Maintain victim and criminal information
* Monitor case progress
* Generate crime-related reports
* Improve investigation efficiency

---

## 🛠️ Technologies Used

* Oracle SQL
* SQL*Plus
* Relational Database Management System (RDBMS)
* ER Modeling

---

## 🗂️ Database Tables

### 1. POLICE_STATION

Stores information about police stations.

Attributes:

* Station_ID (PK)
* Station_Name
* Location

### 2. OFFICER

Stores police officer details.

Attributes:

* Officer_ID (PK)
* Officer_Name
* Rank
* Station_ID (FK)

### 3. VICTIM

Stores victim information.

Attributes:

* Victim_ID (PK)
* Victim_Name
* Age
* Address
* Registered_By (FK)

### 4. CRIMINAL

Stores criminal records.

Attributes:

* Criminal_ID (PK)
* Criminal_Name
* Crime_Level
* Arrested_By (FK)

### 5. CRIME

Stores crime incident details.

Attributes:

* Crime_ID (PK)
* Crime_Type
* Crime_Date
* Victim_ID (FK)
* Criminal_ID (FK)
* Officer_ID (FK)
* Station_ID (FK)

### 6. FIR

Stores First Information Reports.

Attributes:

* FIR_ID (PK)
* Crime_ID (FK)
* Officer_ID (FK)
* FIR_Date

### 7. CASE_FILE

Stores case progress and status.

Attributes:

* Case_ID (PK)
* FIR_ID (FK)
* Officer_ID (FK)
* Case_Status

---

## 🔗 Entity Relationship

Relationships:

* Police_Station → Officer (1:M)
* Officer → Victim (1:M)
* Officer → Criminal (1:M)
* Officer → Crime (1:M)
* Crime → FIR (1:1)
* FIR → Case_File (1:1)

---

## 📊 Features

✔ Crime Record Management

✔ Criminal Information Tracking

✔ Victim Information Management

✔ FIR Registration System

✔ Case Status Monitoring

✔ Officer Performance Reporting

✔ Station-wise Crime Analysis

✔ Crime Investigation Tracking

---

## 📝 SQL Concepts Used

* DDL Commands (CREATE, ALTER)
* DML Commands (INSERT, UPDATE, DELETE)
* Primary Keys
* Foreign Keys
* Joins
* Aggregate Functions
* GROUP BY
* ORDER BY
* Date Functions
* Constraints

---

## 📈 Sample Queries

* List all crimes with victim and criminal names
* Show FIR details with officer and station
* Case status report
* Crimes handled by each officer
* Criminals arrested by each station
* Open and closed cases
* Total FIRs registered
* Crime type analysis
* Officer performance report
* Victim registration report

---

## 📂 Project Structure

Crime-Management-System/

├── README.md

├── CREATE_TABALE_DATA.sql

├── insert_data.sql

├── queries.sql

├── ER_Diagram.png

└── Project_Report.pdf

---

## 🚀 Future Enhancements

* Online FIR Registration Portal
* Criminal Photo Storage
* Fingerprint Verification System
* Web-Based Dashboard
* Crime Prediction Analytics
* Real-Time Reporting System

---

## 📚 Learning Outcomes

Through this project, I gained practical experience in:

* Database Design
* SQL Query Writing
* Database Relationships
* Data Integrity Management
* ER Diagram Design
* Report Generation
* Oracle SQL Development

---

