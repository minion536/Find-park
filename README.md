# Parking Management System

## Overview
The **Parking Management System** is a web-based solution designed to optimize parking space allocation and improve user convenience. The system integrates **IoT sensors** and **web technologies** to allow users to check real-time parking availability, reserve parking spots in advance, and streamline entry/exit processes using QR codes.

## Features
- **User Registration & Login**: Secure authentication system.
- **Real-Time Parking Slot Availability**: View available parking slots dynamically.
- **Reservation System**: Pre-book parking slots for a specific time.
- **QR Code-Based Access**: Scan QR codes for seamless check-in and check-out.
- **Admin Panel**: Manage users, reservations, and parking space availability.
- **Cashless Payment System**: Supports secure online payments.
- **Integration with IoT Sensors**: Real-time monitoring of parking space occupancy.
- **Analytics & Reports**: Generate insights into parking usage trends.

## Tech Stack
### Frontend:
- **HTML, CSS, JavaScript** (for UI design and interactivity)
- **Bootstrap** (for responsive design)

### Backend:
- **PHP** (for business logic and database interactions)
- **MySQL** (for storing user and reservation data)
- **XAMPP** (for local server setup)

### IoT Components:
- **Arduino UNO** (for hardware control)
- **Ultrasonic Sensors** (for detecting parked vehicles)
- **Servo Motors** (for automated barriers)
- **QR Code Scanner** (for user authentication at parking lots)

## System Architecture
1. **User Module**: Allows users to register, log in, and reserve parking slots.
2. **Admin Module**: Provides management controls for parking slots and user data.
3. **IoT Module**: Uses sensors to monitor parking availability in real time.
4. **Database**: Stores user details, parking slot information, and reservation history.

## Installation Guide
### Prerequisites:
- XAMPP (Apache & MySQL)
- Arduino IDE (for IoT programming)
- Web Browser (Chrome/Firefox recommended)

### Steps to Set Up Locally:
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/parking-management-system.git
   ```
2. Start **XAMPP** and enable **Apache & MySQL**.
3. Import the database:
   - Open **phpMyAdmin** (`http://localhost/phpmyadmin`)
   - Create a database named `parking_system`
   - Import the provided `database.sql` file
4. Configure the backend:
   - Open `config.php`
   - Update database credentials if needed:
     ```php
     $host = "localhost";
     $user = "root";
     $password = "";
     $dbname = "parking_system";
     ```
5. Run the project:
   - Place the project folder in `htdocs` (`C:/xampp/htdocs/parking-management-system`)
   - Open `http://localhost/parking-management-system/` in your browser
6. Connect IoT devices:
   - Upload the provided Arduino sketch to the **Arduino UNO**
   - Connect **ultrasonic sensors** and **servo motors** as per the circuit diagram

## Future Enhancements
- Mobile application for easier access
- Integration with **Google Maps** for real-time navigation
- **License Plate Recognition** for automated entry/exit
- **Multiple Slot Booking** and advanced user profiles

## Contributors
- **Mohammed Muzammil Ahmed**
- **Shaik Anwar**

## License
This project is licensed under the [MIT License](LICENSE).

---
Feel free to contribute and enhance the system!

