# TravelFast ✈️🌍  
**A Web-Based Travel Agency Management System**  

## 📌 Overview  
**TravelFast** is a full-stack web application designed to simplify travel bookings, itinerary management, and agency operations. Users can book flights/hotels, manage trips, and agencies can handle inventory via an admin dashboard.  

**Developed by:**  
Kavya Kathiravan, Hailey Hubbard, Jessica Anthonisamy, Rohan Singh, Colton Mazur  

---

## ✨ Key Features  
| Feature                | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| **User Auth**          | Secure registration/login with encrypted passwords.                         |
| **Booking System**     | Book flights/hotels with date validation.                                   |
| **Itinerary Manager**  | View, modify, or cancel bookings in real-time.                             |
| **Payment Processing** | Secure transactions (dummy payment gateway for demo).                       |
| **Admin Dashboard**    | Add destinations, manage bookings, and track revenue.                      |
| **Dynamic Search**     | Filter flights/hotels by destination, date, and budget.                    |

---

## 🛠️ Tech Stack  
**Frontend:**  
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react)  

**Backend:**  
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js)  

**Database:**  
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql)  

**Security:**  
- Parameterized queries (SQL injection prevention)  
- BCrypt password hashing  

---

## 🗄️ Database Schema  
[UML Diagram] https://lucid.app/lucidchart/37f45de6-72c6-43b0-a878-369a49b1c151/edit?invitationId=inv_5fccfc0a-c054-475e-bfa2-2db069657ca9

**Tables:**  
- **`Customer`**: `customerID`, name, username, password  
- **`Booking`**: `bookingID`, _customerID_, bookingDate, bookingType, _flightID/hotelID_, flightClass, checkInDate, checkOutDate, days  
- **`Flight`**: `flightID`, airline, departure/arrival city, departure/arrival time, price, stops
- **`Hotel`**: `hotelID`, hname, location, pricePerNight 
- **`Payment`**: `paymentID`, _bookingID_, totalAmount  

*(1:1 for `Payment`→`Booking`, 1:many for `Customer`→`Booking`)*  

---

## 🚀 Installation  
1. **Clone the repo**  
   ```bash
   git clone https://github.com/janthonii/TravelFast.git
