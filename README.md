This Java-based Bus Booking System is a comprehensive application that demonstrates object-oriented programming principles and Swing GUI development. The system allows passengers to book, manage, and view bus tickets, while administrators can manage schedules and view booking information.

Features
User Features
User Registration & Login:

Two account types: Passenger and Admin

Predefined admin accounts

Username validation (3+ characters, no spaces)

Passenger Functions:

Book seats on available schedules

Cancel existing bookings

Modify seat selections

View personal booking history

Search schedules by route

Admin Functions:

Add new bus schedules

Delete existing schedules

Edit schedule details (route, seats, price)

View all active schedules

View all confirmed bookings

System Capabilities
Data persistence for users, schedules, and bookings

Real-time seat availability tracking

Payment processing simulation (Vodafone Cash/InstaPay)

Input validation for all operations

Clean, responsive GUI with consistent styling

Class Structure
Core Classes
User (Abstract Class)

Base class for all users

Handles authentication and user management

Implements registration and login interfaces

Passenger (Extends User)

Implements passenger-specific functionality

Booking management interface

Admin (Extends User)

Implements admin-specific functionality

Schedule management interface

Schedule

Manages bus schedules

Tracks available seats

Implements Displayable interface

DataStorage

Manages booking data

Handles payment processing simulation

Implements Bookable interface

Support Classes
Main: Entry point of the application

Displayable: Interface for displayable objects

Bookable: Interface for booking operations

File Structure
text
BusBookingSystem/
├── src/
│   ├── User.java               # User management and authentication
│   ├── Passenger.java          # Passenger functionality
│   ├── Admin.java              # Admin functionality
│   ├── Schedule.java           # Schedule management
│   ├── DataStorage.java        # Booking and payment handling
│   ├── Main.java               # Application entry point
│   └── DataStorage/
│       └── Booking.java        # Booking data model
├── data/
│   ├── users.txt               # User database
│   ├── schedules.txt           # Schedule database
│   └── bookings.txt            # Booking database
└── README.md                   # This documentation
How to Run
Ensure you have Java JDK 11+ installed

Compile all Java files:

bash
javac *.java
Run the application:

bash
java Main
Use the following test accounts:

Admin:

Username: admin1, Password: admin123

Username: superadmin, Password: super456

Passenger: Register a new account through the interface

Dependencies
Java SE 11+

Java Swing (included in Java SE)

Java AWT (included in Java SE)

Screenshots
(Screenshots would be added here in an actual GitHub repository)

Main Menu

Login/Registration Screens

Passenger Dashboard

Admin Dashboard

Booking Interface

Schedule Management

Design Patterns
Object-Oriented Programming:

Inheritance (User → Passenger/Admin)

Polymorphism (showMenu() implementation)

Encapsulation (private fields with public getters/setters)

GUI Design:

Model-View separation

Consistent styling with color scheme

Responsive layouts (GridBagLayout, BorderLayout)

Data Persistence:

Text file storage

CSV-like formatting

Automatic loading/saving

License
This project is licensed under the MIT License 
