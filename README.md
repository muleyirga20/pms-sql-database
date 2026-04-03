# 🏥 Patient Management System Database Project

## 📌 Overview

The **Patient Management System** is a SQL Server–based database project designed to manage healthcare data efficiently. It supports storing and retrieving patient information, managing appointments, tracking physicians, and generating reports for decision-making.

This project demonstrates **real-world database design, optimization, and business logic implementation**, making it suitable for portfolio and interview purposes.

---

## 🎯 Objectives

* Design a **normalized relational database**
* Implement **data integrity and constraints**
* Develop **stored procedures and functions**
* Optimize performance using **indexes**
* Support **reporting and analytics**

---

## 🧱 Database Structure

### 📊 Core Tables

* **Patient** – Stores patient personal and demographic information
* **Physician** – Stores doctor details
* **Appointment** – Manages patient appointments
* **MaritalStatus** – Lookup table for marital status
* **AppointmentStatus** *(optional)* – Tracks appointment states

---

## 🔗 Relationships

* One **Patient** → Many **Appointments**
* One **Physician** → Many **Appointments**
* Foreign keys ensure **data consistency and integrity**

## ⚙️ Features Implemented

   ### ✅ Data Integrity
   
    * Primary Keys & Foreign Keys
    * Unique constraints (e.g., Social Security)
    * Check constraints (valid age, etc.)

   ### ⚡ Performance Optimization
   
* Indexes on frequently used columns:

  * `AppointmentDate`
  * `PhysicianID`
* Use of **covering and composite indexes**
   
   ### 🧠 Business Logic
   
   * Prevent double booking of physicians
   * Automatic appointment status handling
   * Data validation in stored procedures
     
## 📦 Stored Procedures

Examples:

* `usp_GetPhysiciansWithMostAppointments`
* `usp_CreateAppointment`
* `usp_GetPatientDetails`

---

## 🔧 User-Defined Functions

### Scalar Functions:

* `ufn_GetPatientAge` → Calculates patient age
* `ufn_GetPatientFullName` → Returns full name
* `ufn_IsPatientActive` → Checks recent activity
* `ufn_GetNextAppointment` → Returns next appointment

---

## 📊 Sample Reports

* Total appointments per day
* Physician workload analysis
* Active vs inactive patients
* Top-performing physicians

---

## 🔐 Transactions & Error Handling

* TRY...CATCH blocks
* Rollback on failure
* Ensures **data consistency in multi-step operations**

---

## 🧪 Testing

* Inserted sample data
* Tested edge cases:

  * Duplicate entries
  * Invalid dates
  * Booking conflicts

---

## 🚀 How to Run

1. Open **SQL Server Management Studio (SSMS)**
2. Create a new database
3. Run scripts in order:

   * Tables
   * Constraints
   * Indexes
   * Functions
   * Stored Procedures
4. Insert sample data
5. Execute queries and procedures

---

## 📁 Project Structure

```
/Tables
/Functions
/StoredProcedures
/Indexes
/Reports
README.md
```

---

## 🏆 Skills Demonstrated

* SQL Server (T-SQL)
* Database Design (Normalization)
* Query Optimization
* Indexing Strategies
* Stored Procedures & Functions
* Error Handling & Transactions

---

## 📌 Future Enhancements

* Integration with **ASP.NET Core application**
* Power BI dashboard for visualization
* Role-based access control (Admin, Doctor, Staff)
* Audit logging and tracking

---

## 👨‍💻 Author

**[Mulugeta Omata]**

* Patient Management System Database Project
* November 11, 2024

## ⭐ Notes

This project is built for **learning, portfolio, and demonstration purposes** and follows best practices used in real-world database systems.
