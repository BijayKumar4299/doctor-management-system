# 🏥 Doctor Management System

A desktop-based **Doctor Management System** developed using Python to help clinics and doctors manage patients, doctors, appointments, consultations, prescriptions, and medical history through a user-friendly graphical interface.

## 📌 Project Overview

The Doctor Management System is designed to simplify common clinic management activities by providing a centralized application for maintaining healthcare records.

The system uses **Tkinter** for the graphical user interface and **SQLite** for local database management. It also supports **PDF prescription generation** using ReportLab and includes email functionality for appointment-related communication.

## ✨ Features

### 🔐 Authentication

* Admin login system
* Username and password management
* Change username
* Change password
* Admin role support

### 👨‍⚕️ Doctor Management

* Add doctors
* Edit doctor information
* Delete doctors
* Search doctors
* Store specialization
* Store phone and email
* Assign consultation room
* Manage doctor availability

### 🧑‍🤝‍🧑 Patient Management

* Register new patients
* Edit patient information
* Delete patients
* Search patients
* Store contact information
* Blood group management
* Allergy information
* Emergency contact
* Patient address
* Patient email
* View patient medical history

### 📅 Appointment Management

* Schedule appointments
* Edit/reschedule appointments
* Search appointments
* Filter appointments by date
* Prevent duplicate doctor appointments
* Process appointments
* Cancel appointments
* Delete appointments
* Appointment status management

### 🩺 Consultation Management

* Record patient symptoms
* Add diagnosis
* Add doctor notes
* Record blood pressure
* Record temperature
* Record weight
* Add follow-up dates
* Maintain consultation history

### 💊 Prescription Management

* Add medicines
* Medicine dosage
* Medicine frequency
* Medicine duration
* Medicine instructions
* Generate prescriptions

### 📄 PDF Generation

* Generate prescription documents
* A4 PDF format
* Structured prescription information
* ReportLab integration

### 📊 Dashboard

The dashboard provides an overview of:

* Total patients
* Total doctors
* Today's appointments
* Completed appointments
* Scheduled appointments
* Cancelled appointments
* Upcoming appointments

## 🛠️ Technologies Used

| Technology        | Purpose                   |
| ----------------- | ------------------------- |
| Python            | Core programming language |
| Tkinter           | Desktop GUI               |
| SQLite            | Database management       |
| ReportLab         | PDF generation            |
| CSV               | Data/file handling        |
| SMTP              | Email communication       |
| Python `datetime` | Date and time management  |

## 🗄️ Database

The application uses **SQLite** with the database file:

```text
doctor_management.db
```

The database contains tables for:

* `users`
* `patients`
* `doctors`
* `appointments`
* `consultations`
* `prescriptions`

Relationships between patients, doctors, appointments, consultations, and prescriptions are maintained using SQLite foreign keys.

## 📂 Project Structure

```text
doctor-management-system/
│
├── Doctor management system(1).ipynb
├── doctor_management.db
└── README.md
```

> The current project is implemented in a Jupyter Notebook. It can later be converted into a standalone Python application with separate modules.

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/BijayKumar4299/doctor-management-system.git
```

### 2. Open the project

Open the notebook:

```text
Doctor management system(1).ipynb
```

using **Jupyter Notebook** or **JupyterLab**.

### 3. Install required packages

Install ReportLab if it is not already installed:

```bash
pip install reportlab
```

The project primarily uses Python standard-library modules such as:

```text
sqlite3
tkinter
csv
os
shutil
datetime
smtplib
email
```

## ▶️ Running the Application

Run the notebook cells in order.

The application can then be started through the project's `main()` function.

The default administrator account configured in the project is:

```text
Username: admin
Password: admin123
```

**For production use, change the default credentials and avoid storing passwords directly in source code.**

## 📧 Email Configuration

The application includes SMTP functionality for sending appointment-related emails.

For security, SMTP credentials should **not** be committed to GitHub.

Use environment variables or another secure configuration method instead.

Example:

```text
SMTP_SERVER = smtp.gmail.com
SMTP_PORT = 465
SMTP_USERNAME = your-email@gmail.com
SMTP_PASSWORD = your-app-password
```

## 🔒 Security Notes

Before deploying this application for real-world use:

* Do not upload passwords to GitHub.
* Do not upload Gmail App Passwords.
* Use password hashing instead of plain-text passwords.
* Keep patient information secure.
* Add proper user roles and permissions.
* Use secure email credentials.
* Add regular database backups.
* Avoid committing real patient information to the repository.

## 🚀 Future Enhancements

Possible future improvements include:

* Modern responsive UI
* Separate Python modules instead of a single notebook
* Secure password hashing
* Multiple user roles
* Doctor availability calendar
* Medicine database with searchable medicines
* Advanced prescription builder
* PDF medical reports
* Automated database backup
* Patient document upload
* Medical report management
* Appointment reminders
* Improved analytics and reports
* Cloud database support
* Web-based version
* REST API integration

## 🎯 Project Objective

The main objective of this project is to create a simple and centralized system that helps manage day-to-day clinic operations while reducing manual record keeping and improving access to patient and appointment information.

## 👨‍💻 Developer

**Bijaya Kumar Sahoo**

GitHub:
https://github.com/BijayKumar4299
