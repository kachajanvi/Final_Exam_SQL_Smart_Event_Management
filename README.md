# Final_Exam_SQL_Smart_Event_Management

# Smart Event Management System

## Project Title

Smart Event Management System

## Author

Janvi Kacha

## Technology Used

- MySQL
- SQL
- Git
- GitHub

## Project Description

The Smart Event Management System is a MySQL-based database project designed to manage events, venues, organizers, attendees, tickets, and payments.

The system helps event organizers manage event information, ticket bookings, payment records, and generate useful reports using SQL queries.

The project demonstrates CRUD operations, filtering, sorting, grouping, aggregate functions, joins, subqueries, date and time functions, string functions, window functions, and CASE expressions.

## Objective

The main objective of this project is to develop a database system that can:

- Manage events and venues
- Manage event organizers
- Manage attendees
- Handle ticket bookings
- Track payment transactions
- Calculate event revenue
- Generate event reports
- Analyze ticket sales
- Apply advanced SQL queries

## Database Name

`smart_event_management`

## Database Tables

The project contains the following tables:

### 1. Venues

Stores information about event venues.

Columns:

- venue_id - Primary Key
- venue_name
- location
- capacity

### 2. Organizers

Stores information about event organizers.

Columns:

- organizer_id - Primary Key
- organizer_name
- contact_email
- phone_number

### 3. Attendees

Stores information about people attending events.

Columns:

- attendee_id - Primary Key
- name
- email
- phone_number

### 4. Events

Stores information about events.

Columns:

- event_id - Primary Key
- event_name
- event_date
- venue_id - Foreign Key
- organizer_id - Foreign Key
- ticket_price
- total_seats
- available_seats

### 5. Tickets

Stores ticket booking information.

Columns:

- ticket_id - Primary Key
- event_id - Foreign Key
- attendee_id - Foreign Key
- booking_date
- status

### 6. Payments

Stores payment information.

Columns:

- payment_id - Primary Key
- ticket_id - Foreign Key
- amount_paid
- payment_status
- payment_date

## Relationships

The database uses Primary Keys and Foreign Keys to establish relationships between tables.

- Events are connected to Venues using `venue_id`.
- Events are connected to Organizers using `organizer_id`.
- Tickets are connected to Events using `event_id`.
- Tickets are connected to Attendees using `attendee_id`.
- Payments are connected to Tickets using `ticket_id`.

## SQL Concepts Used

### CRUD Operations

The project implements:

- INSERT
- SELECT
- UPDATE
- DELETE
- SEARCH

### SQL Clauses

The project uses:

- WHERE
- HAVING
- LIMIT
- ORDER BY
- GROUP BY

### SQL Operators

The project uses:

- AND
- OR
- NOT

### Aggregate Functions

The project uses:

- SUM()
- AVG()
- MAX()
- MIN()
- COUNT()

### Joins

The project demonstrates:

- INNER JOIN
- LEFT JOIN
- RIGHT JOIN
- FULL OUTER JOIN equivalent using UNION

### Subqueries

Subqueries are used to:

- Find events with revenue above average
- Find attendees who booked multiple events
- Find organizers managing multiple events

### Date and Time Functions

The project uses:

- MONTH()
- DATEDIFF()
- DATE_FORMAT()

### String Functions

The project uses:

- UPPER()
- TRIM()
- COALESCE()

### Window Functions

The project uses:

- RANK()
- SUM() OVER()
- COUNT() OVER()

### CASE Expressions

CASE expressions are used for:

- Event demand classification
- Payment status classification

## Main Features

1. Event Management
2. Venue Management
3. Organizer Management
4. Attendee Management
5. Ticket Booking
6. Payment Tracking
7. Revenue Calculation
8. Event Reporting
9. SQL Data Analysis
10. Advanced SQL Queries

## How to Run the Project

### Step 1

Open MySQL or MySQL connection in VS Code.

### Step 2

Open the SQL file:

`event_management.sql`

### Step 3

Run the complete SQL script.

The script will:

1. Delete the existing database if it exists.
2. Create a new database.
3. Create all required tables.
4. Insert sample data.
5. Execute the required SQL queries.

## Project Files

```text
Smart Event Management System
│
├── event_management.sql
└── README.md
