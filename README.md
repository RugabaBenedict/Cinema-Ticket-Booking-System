#  Cinema Ticket Booking System

A lightweight, terminal-based Cinema Ticket Booking System written in **C**. This application manages movie options, seat allocations, real-time ticket transactions, pricing rules, and sales analytics through an interactive command-line interface.

## ✨ Features

- **Interactive Menu**: Easy terminal-based navigation for bookings, searches, updates, and reports.
- **Seat Map Matrix**: Live visual seat map (`[1]`, `[2]`, `[X]`) updated instantly after every transaction to prevent double-booking.
- **Advanced Dynamic Pricing**:
  - **Age Tiers**: Automatic calculations for Child ($5.00), Student ($8.00), and Adult ($12.00).
  - **Weekend Surcharge**: Automatically appends a 20% premium fee for weekend shows.
  - **Group Discount**: Automatically applies a 10% discount for orders of 3 or more tickets.
- **Complete Booking Lifecycle**: Full support to Book, Search, Update (change seats), and Cancel/Delete reservations.
- **Analytics & Summaries**: Identifies the trending "Most Booked Movie" and prints total financial sales/inventory metrics.

---

## 🚀 Preinstalled Movies

The system already has three pre-configured movies, capped at **20 seats** each:
1. `Sci-Fi Odyssey`
2. `The Midnight Mystery`
3. `Animated Adventures`

---

## 🛠️ Getting Started


### What i Used to build the program
To build and run this project, you need a C compiler installed on your system:
- **Windows**: MinGW or GCC via MSYS2
- **macOS**: Xcode Command Line Tools (`clang`)
- **Linux**: GCC (`sudo apt install build-essential`)

### Installation and Compilation

1. **Clone or Download the Repository**
   ```bash
   git clone https://github.com
   cd cinema-booking-system
   ```

2. **Compiling the Code**
   Use `gcc` to compile the source code file (e.g., `main.c`):
   ```bash
   gcc main.c -o cinema_system
   ```

3. **Running the Application**
   - **Linux/macOS**:
     ```bash
     ./cinema_system
     ```
   - **Windows**:
     ```bash
     cinema_system.exe
     ```
---

## 📋 System Menu Overview

When you run the system, you will see the following functional tracks:

```text
=============================================
     CINEMA TICKET BOOKING SYSTEM MENU       
=============================================
1. Book Tickets (Register & Select Seats)
2. Search Bookings
3. Update Booking Details
4. Cancel/Delete Booking
5. Display Available Seats
6. Identify Most Booked Movie
7. Generate Booking Summary & Sales
8. Exit
=============================================
```

---

## ⚙️ Data Build up

The project builds upon two primary `struct` schemas to manage states inside local memory runtime arrays:

- **`Movie` Struct**: Keeps track of the title, individual seat states (0 for available, 1 for occupied), ticket counts, and generated revenue.
- **`Booking` Struct**: Stores customer metadata, allocated unique verification structural IDs (starting at `1001`), customer types (`C`, `S`, `A`), and computed prices.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

