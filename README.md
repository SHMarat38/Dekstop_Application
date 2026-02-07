# E-Shop + CRM (WinForms C#)

## 🛒 About
A **desktop e-commerce application with CRM features**, built with **Windows Forms (C#)** and **MySQL**. This project demonstrates a complete online shopping system with separate interfaces for customers and administrators.

## ✨ Features

### 👤 Customer Side
- **Registration & Login** with SHA256 password hashing
- **Browse catalog** by categories (Laptops, Smartphones, PCs, Tablets)
- **Create orders** from product grid
- **View current order** on main screen
- **Start new order** when needed

### 👑 Admin Panel
- **Separate admin login** with role-based access
- **Full product management** (add/view/delete)
- **User management** (view all users, delete with order cascade)
- **View all orders** in the system
- **Sales monitoring** dashboard

## 🏗️ Tech Stack
- **Platform**: .NET Framework 4.7.2
- **UI**: Windows Forms
- **Database**: MySQL
- **Key Package**: MySql.Data (9.3.0)

## 🚀 Quick Setup

### Prerequisites
1. **Visual Studio 2019+** with .NET 4.7.2
2. **MySQL Server** running locally
3. **Database setup** with tables: `users`, `products`, `categories`, `orders`, `orderitems`

### Configuration
1. **Update connection strings** in all form files (`Form2.cs`, `Form3.cs`, etc.):
```csharp
string connectionString = "server=YOUR_SERVER;user=YOUR_USER;database=YOUR_DB;password=YOUR_PASSWORD;";
```

2. **Restore NuGet packages** (MySql.Data will install automatically)

3. **Build and run** from Visual Studio

## 📱 Application Flow

### Main Forms
1. **Form1** - Landing page with 3 buttons: Login, Register, Admin
2. **Form2** - Customer login
3. **Form3** - Customer registration
4. **Form5** - Admin authentication
5. **Form6** - Main store interface (catalog + orders)
6. **Form7** - Admin dashboard (CRM functions)

### User Journey
```
Registration → Login → Browse Catalog → Select Product → Create Order → View Order
```

### Admin Tasks
- Add/remove products
- Monitor all orders
- Manage user accounts
- View sales data

## ⚠️ Current Limitations
- **One-order-per-user** design (simplified cart system)
- **Hardcoded DB connection** strings (update in each form)
- **Synchronous DB calls** (UI may freeze on slow queries)
- **Basic validation** (needs improvement)

## 🛠️ Architecture Notes

### Security
- Passwords hashed with SHA256 before storage
- Role-based access control (User/Admin)
- Separate login flows for customers and admins

### Database Design
- Relational structure with foreign keys
- Order cascade deletion for data integrity
- Category-based product organization

## 📝 Project Status
**This is a learning project** - it demonstrates core concepts but needs refinement for production use. Great for understanding WinForms + MySQL integration, basic e-commerce workflows, and simple CRM functionality.

---

*Note: Developed as a course project. Code is open for educational purposes. Feel free to adapt and improve!*
