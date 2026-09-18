# JAVA-PROJECT
# 🎬 Movie Ticket Booking System (Java)

A console-based **Movie Ticket Booking System developed in Java** that simulates a real-world movie ticket booking process. The system allows customers to view movie details, check seat availability, and book movie tickets while demonstrating important **Object-Oriented Programming (OOP)** concepts.

---

## 📌 Features

* 🎥 View movie details
* 💺 Display available seats
* 🎟️ Book movie tickets
* ✅ Booking confirmation
* 🔄 Seat availability management
* 📧 Email validation
* 📋 Menu-driven console interface
* 👨‍💼 Admin and Customer roles
* 🛡️ Duplicate booking prevention
* ⚠️ Invalid input and seat validation
* 🧩 Implementation of OOP concepts

---

## 🛠️ Technologies Used

* **Java**
* **Object-Oriented Programming (OOP)**
* **Collections Framework**
* **Scanner Class**
* **Console-Based User Interface**

---

## 📂 Project Structure

The complete project is implemented in a single Java file:

```text
Movie_Ticket_Booking_System.java
```

### Classes Used

| Class                         | Description                               |
| ----------------------------- | ----------------------------------------- |
| `User`                        | Base class for all users                  |
| `Admin`                       | Handles administrator operations          |
| `Customer`                    | Handles customer operations               |
| `Movie`                       | Stores movie details                      |
| `Theater`                     | Manages theater and movies                |
| `Seat`                        | Manages individual seat information       |
| `Show`                        | Handles movie shows and seat availability |
| `Booking`                     | Stores booking information                |
| `BookingService`              | Handles ticket booking logic              |
| `Movie_Ticket_Booking_System` | Main class used to run the application    |

---

## 🧠 OOP Concepts Used

### 1. Encapsulation

Encapsulation is implemented by keeping class variables private and providing appropriate **getters and setters** to access and modify them.

**Example:**

```java
private String name;

public String getName() {
    return name;
}

public void setName(String name) {
    this.name = name;
}
```

---

### 2. Inheritance

Inheritance allows one class to acquire the properties and methods of another class.

In this project:

```text
              User
             /    \
         Admin   Customer
```

Both `Admin` and `Customer` inherit from the `User` class.

---

### 3. Polymorphism

Polymorphism is demonstrated through **method overriding**.

For example, the `performRole()` method can be overridden by different user types:

```java
Admin
Customer
```

Each class can provide its own implementation of the method.

---

### 4. Abstraction

The booking-related operations are separated from the user interface through the `BookingService` class.

This helps keep the booking logic organized and makes the system easier to maintain and extend.

---

## 🔄 System Workflow

```text
              START
                │
                ▼
       Display Main Menu
                │
        ┌───────┴────────┐
        ▼                ▼
   View Movie        Book Ticket
        │                │
        ▼                ▼
 Movie Details      Enter User Details
                         │
                         ▼
                  Validate Email
                         │
                         ▼
                 Display Available Seats
                         │
                         ▼
                  Select Seat
                         │
                         ▼
                Check Seat Availability
                    │           │
                   No          Yes
                    │           │
                    ▼           ▼
              Show Error    Book Seat
                                │
                                ▼
                       Booking Confirmation
                                │
                                ▼
                              EXIT
```

---

## ▶️ How to Run

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Java-Projects-Collections.git
```

### Step 2: Navigate to the Project Directory

```bash
cd Java-Projects-Collections
```

Navigate to the Movie Ticket Booking System project folder if required.

### Step 3: Compile the Java Program

```bash
javac Movie_Ticket_Booking_System.java
```

### Step 4: Run the Program

```bash
java Movie_Ticket_Booking_System
```

---

## 📋 Sample Menu

```text
========================================
       MOVIE TICKET BOOKING SYSTEM
========================================

1. View Movie
2. Book Ticket
3. Exit

Enter your choice:
```

---

## 🎟️ Sample Booking Flow

```text
===== MOVIE TICKET BOOKING SYSTEM =====

Enter your name: JOHN
Enter email: john@gmail.com

Available Seats:
A1
A2
A3
A4
A5

Enter seat number: A1

Seat booked successfully!

========================================
          BOOKING CONFIRMED
========================================
Customer Name : JOHN
Email         : john@gmail.com
Seat Number   : A1
========================================
```

---

## 🔐 Validations Implemented

The system performs several validations to prevent invalid operations.

### 📧 Email Validation

Checks whether the entered email follows a valid email format.

### 💺 Seat Availability Checking

Before booking, the system checks whether the selected seat is available.

### 🚫 Duplicate Booking Prevention

A seat that has already been booked cannot be booked again.

### ⚠️ Invalid Seat Handling

The system displays an error message when the user enters an invalid seat number.

### ⏱️ Duration Validation

Invalid movie/show duration values are handled through validation.

---

## 📦 Collections Framework

The project uses Java's **Collections Framework** to efficiently manage data such as movies, seats, shows, and bookings.

Collections make it easier to:

* Store multiple objects
* Search for available seats
* Add or remove bookings
* Manage movie and show information

---

## 👥 User Roles

### 👨‍💼 Admin

The Admin role is designed to handle administrative operations such as managing movie-related information and system data.

### 👤 Customer

The Customer role allows users to:

* View movies
* Check available seats
* Enter booking information
* Select seats
* Book tickets
* Receive booking confirmation

---

## 🚀 Future Enhancements

The current console-based application can be extended with several advanced features:

* 🗄️ Database integration using MySQL
* 🖥️ GUI implementation using Java Swing or JavaFX
* 🎬 Support for multiple movies and shows
* 💳 Payment gateway simulation
* ❌ Ticket cancellation
* 🔐 User authentication and login
* 📱 Responsive web or mobile interface
* 🧾 Digital ticket generation
* 📧 Email confirmation
* ⭐ Movie rating and review system
* 🔍 Movie search and filtering

---

## 🎯 Project Objectives

The main objectives of this project are:

1. To develop a basic movie ticket booking application using Java.
2. To understand and implement **Object-Oriented Programming concepts**.
3. To demonstrate inheritance, encapsulation, polymorphism, and abstraction.
4. To manage seat availability and prevent duplicate bookings.
5. To implement input validation.
6. To understand the use of Java Collections.
7. To create a simple menu-driven console application.

---

## 📚 Learning Outcomes

After completing this project, the developer gains practical understanding of:

* Java classes and objects
* Constructors and methods
* Encapsulation
* Inheritance
* Polymorphism
* Abstraction
* Method overriding
* Java Collections
* User input using `Scanner`
* Input validation
* Basic software design
* Console-based application development
