#  Supply Chain Database Case Study
# Overview
This project demonstrates the development, management, and utilization of a Supply Chain Database to track products from suppliers to customers, optimize inventory management, and streamline logistics. The database tracks key data such as product information, supplier details, inventory levels, shipments, and customer orders.

The project uses MySQL as the database management system and Python for automation and integration tasks. The database schema is version-controlled using GitHub, allowing seamless collaboration and sharing of scripts and reports.

# Project Objectives
The goal of this project was to build a centralized, scalable database to:

Track the movement of products through various stages of the supply chain.
Improve inventory management and reduce stockouts.
Optimize logistics by tracking delivery times and costs.
Improve decision-making through better data visibility and analysis.

# Components
1. Products Table
Stores information about products including name, SKU, description, category, and supplier.

ProductID: Unique identifier for the product.
ProductName: Name of the product.
SupplierID: Foreign key referring to the Supplier table.
Category: Product category (e.g., electronics, appliances).
UnitPrice: Price of a single unit of the product.

2. Suppliers Table
Contains data about suppliers, such as company name, location, and contact details.

SupplierID: Unique identifier for the supplier.
SupplierName: Name of the supplier.
ContactPerson: Primary contact person at the supplier.
Country: Country where the supplier is based.

3. Inventory Table
Tracks the quantities of products in various warehouses, as well as historical stock data.

WarehouseID: Unique identifier for the warehouse.
ProductID: Foreign key referring to the Products table.
Quantity: Quantity of product currently in stock.
LastUpdated: Timestamp of when the stock level was last updated.

4. Orders Table
Stores customer order information including order date, total amount, and shipping address.

OrderID: Unique identifier for the order.
CustomerID: Foreign key referring to the Customers table.
OrderDate: Date the order was placed.
TotalAmount: Total value of the order.
ShippingAddress: Delivery address for the order.

5. Shipments Table
Tracks shipments, delivery status, and associated order information.

ShipmentID: Unique identifier for the shipment.
OrderID: Foreign key referring to the Orders table.
ShipmentDate: Date the shipment was sent.
DeliveryStatus: Current status of the shipment (e.g., in transit, delivered).
TrackingNumber: Carrier tracking number for the shipment.

6. Customers Table
Stores customer information, including billing and shipping addresses.

CustomerID: Unique identifier for the customer.
CustomerName: Full name of the customer.
ContactEmail: Customer’s email address.
Address: Customer’s billing/shipping address.

7. Logistics Table
Contains logistics-related data, including transport methods and delivery costs.

LogisticsID: Unique identifier for the logistics record.
ShipmentID: Foreign key referring to the Shipments table.
Carrier: The logistics provider handling the shipment.
TransportMode: Method of transportation (e.g., air, sea, land).
Cost: Shipping cost associated with the shipment.

# Technologies Used
Database Platform: MySQL (Relational database for storing and managing supply chain data)
Programming Language: Python (for automation, data processing, and API integration)
Data Analysis Tools: Tableau/Power BI (for creating reports and dashboards)
Version Control: GitHub (for collaboration, versioning, and code management)

# Installation and Setup
Prerequisites
Install MySQL on your system.

Download MySQL from: MySQL Downloads
Install Python 3.x and required libraries:

Install Python from: Python Downloads
Install necessary Python libraries using pip:

# License
This project is licensed under the MIT License – see the LICENSE file for details.

# Acknowledgements
MySQL for providing a robust database platform.
Python for automation and handling data processing.
Power BI/Tableau for data visualization and reporting.
GitHub for version control and collaboration.
