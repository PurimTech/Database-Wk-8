# 📦 E-commerce Database (MySQL)

## 📌 Objective
This project is a **relational database schema for an E-commerce Store**, implemented using MySQL.  
It demonstrates the use of **tables, constraints, and relationships** (one-to-one, one-to-many, many-to-many).

---

## 🛠️ Features
- Manage **Users** (customers with unique accounts)
- Manage **Products** and organize them into **Categories**
- Handle **Orders** and **Order Items**
- Record **Payments** for orders
- Manage **Shopping Cart** functionality

---

## 🗂️ Database Schema
### Entities:
1. **Users** – Stores customer information.  
2. **Categories** – Groups of products (e.g., Electronics, Fashion).  
3. **Products** – Items available for sale.  
4. **Orders** – Customer orders with status tracking.  
5. **Order_Items** – Links orders to products (Many-to-Many).  
6. **Payments** – Stores order payment details.  
7. **Cart** – Temporary cart storage before checkout.

---

## 🔑 Relationships
- **Users → Orders**: One-to-Many  
- **Categories → Products**: One-to-Many  
- **Orders → Order_Items → Products**: Many-to-Many  
- **Orders → Payments**: One-to-One  
- **Users → Cart (Products)**: One-to-Many  

---

## 🏗️ How to Use
1. Open MySQL Workbench or MySQL CLI.
2. Run the provided `ecommerce.sql` script:
   ```sql
   SOURCE ecommerce.sql;
