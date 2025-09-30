# ERD-Kiwilytics-Project

## 📌 Project Overview
This project contains the database design and Entity-Relationship Diagram (ERD) for a retail/order management system. The design includes tables, primary keys, foreign keys, and relationships that demonstrate how data is structured and connected in a relational database

## 🗂️ Database Tables
The database includes the following entities:
- **Categories**
- **Customers**
- **Employees**
- **Orders**
- **Order_Details**
- **Products**
- **Shippers**
- **Suppliers**

## 🔑 Keys
### Primary Keys
- **Categories** → `CategoryID`
- **Customers** → `CustomerID`
- **Employees** → `EmployeeID`
- **Orders** → `OrderID`
- **Order_Details** → `(OrderID, ProductID)` (composite key)
- **Products** → `ProductID`
- **Shippers** → `ShipperID`
- **Suppliers** → `SupplierID`

### Foreign Keys
- **Orders**
  - `CustomerID` → Customers(CustomerID)
  - `EmployeeID` → Employees(EmployeeID)
  - `ShipperID` → Shippers(ShipperID)
- **Order_Details**
  - `OrderID` → Orders(OrderID)
  - `ProductID` → Products(ProductID)
- **Products**
  - `CategoryID` → Categories(CategoryID)
  - `SupplierID` → Suppliers(SupplierID)

## 📊 ERD Diagram

<img width="1563" height="764" alt="ERD" src="https://github.com/user-attachments/assets/c5d009e5-f9c9-4a75-ac6d-189011b4fab8" />

## 🎯 Use Cases
This database schema can support multiple business scenarios. Examples include:

1. **Retail / E-Commerce Platform**  
   - Manage customers, orders, products, and suppliers.  
   - Track shipments and stock levels.  
   - Generate reports on sales, revenue, and product performance.  

2. **Inventory & Supply Chain Management**  
   - Monitor product categories, suppliers, and stock availability.  
   - Record shipments handled by different shippers.  
   - Calculate inventory turnover rates.  


