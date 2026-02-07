# Secure E-Commerce & CRM System (C# WinForms + MySQL)

![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![.NET Framework](https://img.shields.io/badge/.NET%20Framework%204.7.2-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)

## 📌 Project Overview
This project is a comprehensive desktop application designed as a course work for the **"Object-Oriented Programming"** discipline at the **National Aviation Academy (Azerbaijan)**. It serves as a prototype for an e-commerce platform and CRM system, focusing on secure data management and relational integrity.

## 🛠 Features

### 🔐 Security & Access Control
- **SHA-256 Hashing:** User passwords are cryptographically hashed before being stored in the database to ensure high-level security.
- **Role-Based Access:** Separate authentication flows and interfaces for **Customers** and **Administrators**.
- **SQL Injection Prevention:** Utilization of parameterized queries to protect the database from unauthorized manipulation.

### 💻 Functionality
- **Dynamic Catalog:** Browsing products categorized into groups such as Laptops, PCs, Smartphones, and Tablets.
- **Transaction Management:** Real-time order creation and storage linked to user accounts.
- **Admin Dashboard:** Full CRUD (Create, Read, Update, Delete) operations for inventory and user management.

## 🏗 System Architecture
The application follows a client-server model:
- **Frontend:** Developed in C# using the **Windows Forms** (WinForms) environment.
- **Backend:** **MySQL Server** for centralized data storage with a relational schema (5 tables: `users`, `products`, `categories`, `orders`, `orderitems`).

## 📂 Project Structure
- `DB.cs`: Centralized database connection management.
- `Form1.cs` to `Form7.cs`: UI modules for authentication, shop catalog, and administrative controls.
- `Security/`: Implementation of SHA-256 hashing logic.

## ⚙️ Installation
1. Clone the repository.
2. Import the provided SQL dump into your MySQL Server.
3. Update the `connectionString` in the source code with your local DB credentials.
4. Build and run via Visual Studio 2019/2022.

---
**Course Work Author:** Marat Shirinov  
**Institution:** National Aviation Academy, Baku 2025
