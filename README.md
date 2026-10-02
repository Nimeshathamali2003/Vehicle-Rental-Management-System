# 🚗 Vehicle Rental Management System

A database-driven application designed to manage the daily operations of a vehicle rental business.

---

## 📋 About the Project

The Vehicle Rental Management System is a database-driven application designed to manage the daily operations of a vehicle rental business. The system stores and manages information related to **customers, vehicles, bookings, and payments**.

This project focuses on designing a well-structured relational database using **DBMS concepts** such as entities, relationships, normalization, and SQL queries.

---

## 🎯 Aim

To design and implement a relational database for a Vehicle Rental Management System that efficiently manages customer details, vehicle information, bookings, and payments.

---

## 🎯 Objectives

- To design a structured relational database for a vehicle rental system
- To store and manage customer and vehicle information efficiently
- To handle vehicle booking and payment records accurately
- To reduce data redundancy using normalization techniques
- To apply DBMS concepts such as primary keys, foreign keys, and SQL queries

---

## 🛠️ Tools and Technologies Used

| Component | Technology |
|-----------|-----------|
| **Database Management System** | MySQL |
| **Query Language** | SQL |
| **Design Tools** | ER Diagram (draw.io / Lucidchart) |
| **Platform** | Windows |

---

## 🗄️ Database Design (4 Tables)

### 1. Customer Table
- `customer_id` (Primary Key)
- `name`
- `nic`
- `phone`
- `email`
- `address`

### 2. Vehicle Table
- `vehicle_id` (Primary Key)
- `vehicle_number`
- `type`
- `brand`
- `model`
- `year`
- `rent_per_day`
- `status`

### 3. Booking Table
- `booking_id` (Primary Key)
- `customer_id` (Foreign Key)
- `vehicle_id` (Foreign Key)
- `start_date`
- `end_date`
- `total_days`
- `total_amount`
- `booking_status`

### 4. Payment Table
- `payment_id` (Primary Key)
- `booking_id` (Foreign Key)
- `payment_date`
- `amount`
- `payment_method`

---

## 🔗 Primary Keys and Foreign Keys

**Primary Key:** A column that uniquely identifies each record (row) in a table.
- Cannot be NULL
- Cannot have duplicate values
- Example: `customer_id` in the Customer table

**Foreign Key:** A column that links one table to another table.
- Refers to the Primary Key of another table
- Purpose: To keep data connected and accurate
- Example: `customer_id` in the Booking table refers to `customer_id` in the Customer table

---

## 📊 Diagrams

### Entity Relationship (ER) Diagram

The system has **Customer**, **Vehicle**, **Booking**, and **Payment** entities.

- A Customer can make many Bookings.
- A Vehicle can be booked many times.
- Each Booking belongs to one Customer and one Vehicle.
- Each Booking has Payment details.
- Primary Keys uniquely identify records.
- Foreign Keys connect related tables.

### Class Diagram

- **Customer** class stores customer details and is connected to the **Booking** class.
- Each **Booking** is associated with one **Vehicle**.
- Every booking has a corresponding **Payment**.

### Use Case Diagram

- **Customer:** Register/Login, View Available Vehicles, Make a Booking, Make a Payment
- **Admin:** Manage Customers, Manage Vehicles, Manage Bookings, Manage Payments

---

## ✨ Key Features

- ✅ Stores and manages customer details efficiently
- ✅ Maintains complete vehicle information and availability status
- ✅ Handles vehicle booking records accurately
- ✅ Records and manages payment details securely
- ✅ Uses primary and foreign keys to maintain data integrity
- ✅ Reduces data redundancy through normalization
- ✅ Enables quick and easy data retrieval using SQL queries
- ✅ Provides a centralized database for all rental operations

---

## ⚠️ Problem Statement

Many vehicle rental companies still rely on manual or semi-computerized methods to manage customer records, vehicle details, bookings, and payments. These traditional systems lead to:

- Data redundancy
- Booking conflicts
- Inaccurate billing
- Difficulty in tracking vehicle availability

As the volume of data increases, managing and retrieving information becomes time-consuming and error-prone. Therefore, there is a need for a well-structured database system that can efficiently store, manage, and retrieve vehicle rental information while ensuring data accuracy, consistency, and reliability.

---

## ✅ Proposed Solution

A **centralized Vehicle Rental Management System** using a relational database that:

- Stores customer, vehicle, booking, and payment information in well-structured tables
- Uses proper primary and foreign keys
- Applies normalization techniques to reduce data redundancy
- Allows efficient tracking of vehicle availability
- Provides accurate booking management and reliable payment records

This computerized database solution improves data accuracy, simplifies data retrieval, and enhances overall efficiency in vehicle rental operations.

---

## 📌 Scope of the Project

This project covers the following functionalities:

- Managing customer details
- Managing vehicle details and availability
- Recording booking information
- Storing payment details
- Generating basic reports using SQL queries

---

## 🚀 How to Run

1. Install **XAMPP**
2. Open **phpMyAdmin** (`http://localhost/phpmyadmin`)
3. Create a new database named `vehicle_rental_db`
4. Import the `vehicle_rental_db.sql` file
5. Run SQL queries to view and manage data

---

## 📅 Project Schedule

| Activity | Duration |
|----------|----------|
| Project Initiation | Week 1 |
| Project Planning | Week 2 |
| Design Phase | Week 3-4 |
| Development Phase | Week 5-8 |
| Documentation | Week 9-10 |
| Final Presentation and Viva | Week 11-12 |

---

## 👩‍💻 Author

**U.G. Nimesha Thamali**

- **Reg No:** TAN/IT/2324/F/0044
- **Institution:** SLIATE – Advanced Technical Institute, Tangalle
- **Email:** nimeshathamali151@gmail.com
- **Supervisor:** Mr. G.R.C. Kumara

---

## 📚 References

- Odoo Apps Store – Vehicle Rental Management System
- Nizi Solutions – Car Rental Software in Colombo, Sri Lanka
- RentSyst – Car Rental Software
- FleetON – Car Rental Management System Solution
- CoastR – All-In-One Car Rental Software

---

## 📄 License

This project is submitted for the partial fulfillment of **HNDIT 3042 – Database Management Systems Project** at SLIATE – Advanced Technical Institute, Tangalle.
