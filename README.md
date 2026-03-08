# Booking App

This is a CLI booking application I developed based on an online course to practice Go fundamentals and understand how core language features work together in a small project.

The project focuses on learning and applying:
- Variables & Constants in Go  
- Formatted Output (`Printf`)  
- Data Types in Go  
- Getting User Input  
- Pointers  
- Arrays & Slices  
- Loops  
- Conditionals (`if / else`) and Boolean values  
- Input Validation  
- Switch Statements  
- Functions  
- Package Organization  
- Scope Rules  
- Maps  
- Structs  
- Goroutines and Concurrency  
- WaitGroups for synchronization  

## Project Overview

This application simulates a conference ticket booking process directly in the terminal.

Users are asked to provide:

- First name  
- Last name  
- Email address  
- Number of tickets to book  

After validating the information, the booking is stored in memory and the remaining number of tickets is updated.

A confirmation ticket is then sent asynchronously using a goroutine to simulate background processing.

## Main Features

- Interactive terminal input  
- Ticket availability tracking  
- Validation of user data  
- In-memory booking storage  
- Struct-based user information  
- Goroutine execution for asynchronous tasks  
- WaitGroup synchronization to control concurrent execution  

## Validation Rules

The application validates the following conditions before accepting a booking:

- First name must contain at least 2 characters  
- Last name must contain at least 2 characters  
- Email must contain `@`  
- Requested tickets must be greater than zero  
- Requested tickets cannot exceed the remaining available tickets  

## Project Structure

```text
booking-app/
│── main.go
│── go.mod
│── README.md
│── helper/
│   └── helper.go
```

## How to Run

Make sure Go is installed on your machine, then execute:

```bash
go run .
```