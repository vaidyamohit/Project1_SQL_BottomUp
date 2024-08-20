# Project1_SQL_BottomUp- Maruti Suzuki

## Overview
This project demonstrates the design and implementation of a relational database for a vehicle management system(Maruti Suzuki). Using a top-down approach, the database structure focuses on key aspects of the system such as customer management, vehicle inventory, sales, service records, dealerships, and supplier information. The project involves creating several interconnected tables to efficiently store and retrieve data related to vehicle sales and service operations.

## Approach

This project utilizes a bottom-up approach to database design. We started by identifying and defining the detailed attributes and relationships of specific data elements within the vehicle management system(Maruti Suzuki). By gradually integrating these elements into larger, more complex entities and processes, we constructed a cohesive and well-structured database. This method ensured that all foundational data components were thoroughly considered and accurately represented, resulting in a robust system that effectively supports vehicle sales, service, and inventory management.

## Project Structure

The project is structured around the following main entities:

1. **Customers**: Stores customer information, including CustomerID, Name, Email, PhoneNumber, and Address.
2. **Vehicles**: Contains details about vehicles such as VehicleID, ModelName, VIN, Price, and ManufactureDate.
3. **Sales**: Tracks sales transactions, including SaleID, CustomerID, VehicleID, SaleDate, DealershipID, and TotalAmount.
4. **Dealerships**: Stores information about dealerships with fields like DealershipID, DealershipName, Address, and PhoneNumber.
5. **ServiceCenters**: Manages service center details with ServiceCenterID, ServiceCenterName, Address, and PhoneNumber.
6. **ServiceRecords**: Keeps track of vehicle service records, including ServiceRecordID, VehicleID, ServiceCenterID, ServiceDate, ServiceDetails, and Cost.
7. **Employees**: Maintains employee information such as EmployeeID, Name, Position, DealershipID, ServiceCenterID, Email, and PhoneNumber.
8. **Parts**: Manages inventory of parts with PartID, PartName, VehicleID, Price, StockQuantity, and SupplierID.
9. **Suppliers**: Stores supplier information including SupplierID, SupplierName, Address, PhoneNumber, and Email.

## Database Schema

The database schema includes the following tables:

- Customers
- Vehicles
- Sales
- Dealerships
- ServiceCenters
- ServiceRecords
- Employees
- Parts
- Suppliers

Each table is designed with appropriate fields and data types to ensure efficient data storage and retrieval.

## Relationships

The database schema includes the following key relationships:

1. Customers to Sales: One-to-Many
2. Vehicles to Sales: One-to-Many
3. Dealerships to Sales: One-to-Many
4. Vehicles to ServiceRecords: One-to-Many
5. ServiceCenters to ServiceRecords: One-to-Many
6. Dealerships to Employees: One-to-Many
7. ServiceCenters to Employees: One-to-Many
8. Vehicles to Parts: One-to-Many
9. Suppliers to Parts: One-to-Many

## Roles and Permissions

The system can include various user roles with different levels of access:

1. Administrator: Full access to all tables and data
2. Sales Representative: Manage customer information and sales records
3. Service Technician: Access and update service records
4. Inventory Manager: Manage vehicle and parts inventory
5. Human Resources: Manage employee information
6. Finance Officer: Access to sales and cost information
7. Customer Service Representative: View customer, vehicle, and service information
8. Auditor: Read-only access to all tables for audit purposes

Each role should have specific permissions designed to ensure data security and maintain the principle of least privilege.

## Contributors

Diksha Jain - 045018
Mohit Vaidya - 045032
Shantanu Bharvirkar - 045052
