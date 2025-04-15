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
![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat&logo=angular) *(Choose one)*  

**Backend:**  
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=spring-boot)  
*(OR)* ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js)  

**Database:**  
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql)  

**Security:**  
- Parameterized queries (SQL injection prevention)  
- BCrypt password hashing  

---

## 🗄️ Database Schema  
![UML Diagram] https://lucid.app/lucidchart/37f45de6-72c6-43b0-a878-369a49b1c151/edit?invitationId=inv_5fccfc0a-c054-475e-bfa2-2db069657ca9

**Tables:**  
- **`customer`**: `customerID`, name, username, password  
- **`booking`**: `bookingID`, `customerID`, `flightID`/`hotelID`, dates  
- **`flight`**: `flightID`, airline, departure/arrival cities  
- **`hotel`**: `hotelID`, name, location, price  
- **`payment`**: `paymentID`, `bookingID`, total amount  

*(1:1 for `payment`→`booking`, 1:many for `customer`→`booking`)*  

---

## 🚀 Installation  
1. **Clone the repo**  
   ```bash
   git clone https://github.com/your-username/TravelFast.git
