Car Rental System
----------------------------------------------------------------------------------------

**Introduction**

The Car Rental System is a web-based application designed to simplify and streamline car rental operations. It enables customers to browse available vehicles, make reservations, and rent cars for specific durations. Meanwhile, rental companies can efficiently manage their fleet, customer records, and bookings.

**Business Domain Description**

Description

The Car Rental System is a comprehensive platform for managing vehicle fleets, tracking rentals, generating invoices, and maintaining customer records. It offers an intuitive interface for both customers and administrators.

**Key Features**

Vehicle Management:

Add, view, and manage rental vehicles.

Customer Management:

Manage customer accounts, rental history, and personal information.

Rental Reservation:

Customers can search for available vehicles and make reservations based on specific criteria.

Booking and Payment:

Calculate rental fees based on vehicle type, rental duration, and services. Supports payments via Google Pay, PayPal, and bank transfer.

**Use Cases**

1. Adding a Vehicle

Steps:

Enter vehicle details (make, model, year, registration number, etc.).

System updates the fleet database.

2. Customer Reservation

Steps:

Browse available vehicles based on location, date range, and vehicle type.

Select a vehicle and provide booking details (pickup/drop-off locations, rental duration).

3. User Creation

Steps:

Create a new user account using a valid email and password.

Business Objects
Car Data
Attributes: Brand, Model, Year, Color, Type, Fuel, Transmission, Rental Price

Operations: Add new vehicles, Display all vehicles

Bookings
Attributes: Reference Number, Name, Email, Mobile, Pickup/Drop-off Details, Payment

Operations: Add new bookings

User Registration
Attributes: Email, Password, Active status

**System Overview**

Design
Frontend Components
Multiple HTML templates: index.html, about.html, register.html, login.html, cars.html, booking.html

Rendered using Flask for dynamic content

Backend Components

Flask: Handles server-side logic and HTTP requests

MongoDB: Stores car data, user information, and bookings (accessed via pymongo)

User Registration & Authentication: Supports account creation, login, and verification

Car Data Management: Insert and retrieve vehicle information

Booking Management: Book cars and generate unique reference numbers for each booking

Overall Architecture
Follows a client-server model

Flask serves as the backend

MongoDB handles data storage

Frontend communicates with the backend via HTTP requests

User Interface
Homepage (index.html)
Navigation bar for easy access to all sections

Search and filter options for cars

About Page (about.html)
Information about the company, mission, and vision

Registration (register.html) & Login (login.html)
User-friendly forms for account creation and login

Validation and error handling

Car Listing Page (cars.html)
Displays all available cars with detailed information

Sorting and filtering options

Booking Page (booking.html)
Step-by-step booking process

Booking summary displayed before confirmation

User Experience (UX)
Clear and simple registration and login process

Organized car listing with filters

Intuitive booking process with clear instructions and validation

**Conclusion**

The Car Rental System is a complete web solution built with Flask and MongoDB to efficiently manage car rentals. It provides essential features like user registration, car listings, bookings, and seamless payment integration, enhancing the rental process for both customers and rental companies.
