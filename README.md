# Integrated Exam Hub: QR Code Hall Ticket & Fingerprint Attendance System

**Integrated Exam Hub** is a secure, two-step exam verification platform integrating a **web portal** and a **mobile application**, both connected to a unified backend.  
It is designed to modernize the examination process in educational institutions by automating hall allocation, improving authentication, and ensuring fairness and accessibility for all students.

This repository contains documentation and selected components of the project.  
The full implementation (including backend logic and biometric modules) is proprietary and not publicly shared.

---

## 🔹 Project Overview
The **Integrated Exam Hub** simplifies and secures the entire exam lifecycle — from hall allocation and staff scheduling to student authentication and attendance tracking.  
It enhances operational efficiency while ensuring inclusivity, transparency, and academic integrity.

---

## ⚙️ Features

### 🧮 Dynamic Hall Allocation
- 📅 Automatically generates **timetables for each course**.  
- 🏫 Schedules **exam rooms** for each session (with date and time).  
- 🎓 Allocates **students to rooms** based on their registered exams and seat numbers.  
- ♿ Ensures **inclusive access**:  
      ➜ Students with disabilities are prioritized for first-floor rooms (as lifts or ramps may be unavailable, inaccessible, or not functional in many colleges).  
- 👩‍🏫 After student allocation, assigns **staff invigilators** to each room and session.  
- 🎟️ Generates **digital hall tickets** for students and displays staff schedules (date, time, and assigned exam hall) on their dashboards.

---

### 🔐 Two-Step Verification (QR Code + Fingerprint)
- Combines **QR Code** and **Fingerprint Scanning** for secure and verified student check-ins.  

- **QR Code Hall Ticket:**  
  ➜ Each student’s QR code contains essential details such as **Subject ID**, **Subject Name**, **Exam Date**, **Session**, **Hall Name**, **Building**, and **Seat Number**.  
  ➜ Scanning the QR code retrieves the student’s details directly from the web portal.  

- **Fingerprint Verification:**  
  ➜ Accessible **only to staff** through the mobile app.  
  ➜ Each student’s fingerprint is securely stored and hashed in the database.  
  ➜ Invigilator enters the **Student ID** → scans the fingerprint → system verifies against stored data.  
  ➜ If the fingerprint matches, a **“Verification Success”** message appears.  
  ➜ Both QR and fingerprint checks happen seamlessly within the app for quick identity validation.

---

### 🖥️ Dashboards (Separate for Students & Staff)
- **Dedicated login portals** for each role.  
- **Two-step login verification:**  
  ➜ Student/Staff ID + Password  
  ➜ OTP sent to the registered college email ID (Both the ID and email ID are stored in the database, and the dashboard opens only when they are verified as correct.)
  
- **Student Dashboard:**  
  ➜ Download hall tickets.  
  ➜ View exam schedules and venues.  

- **Staff Dashboard:**  
  ➜ View invigilation assignments by date and session.  
  ➜ Access student verification data and exam details.

---

### 🔔 Real-Time Exam Alerts
- Sends **exam notifications and venue details** via **email**.  
- *(Planned update: WhatsApp integration for faster alerts.)*

---

### 🔒 Secure Data Handling
- 🔑 Passwords are **hashed** before storing — even admins cannot view them.  
- 🧬 **Biometric data (fingerprints)** are securely encrypted and used only for authentication.  
- ✅ Complies with privacy and data security standards.

---

## 🔹 Technologies Used

### 🖥️ Web Application
- **Language:** Python  
- **Framework:** Flask  
- **Frontend:** HTML, CSS, JavaScript  
- **Database:** MySQL  
- **Libraries & Modules:**
  - Flask-Mail – for sending OTPs via email  
  - ReportLab – for generating PDF hall tickets  
  - qrcode – for QR code generation  
  - dotenv – for environment variable management  
  - werkzeug – for password hashing and security  
  - flask_cors, flask_logging – for CORS and access log handling  

---

### ⚙️ Backend Integration (Connector)
- **Language:** PHP  
- **Server:** WAMP (Apache + MySQL + PHP)  
- **Purpose:** Acts as a bridge between mobile app and backend database  
- **Libraries & Features:**
  - PDO – for secure MySQL connection  
  - JSON handling – for API communication  

---

### 📱 Mobile Application
- **Platform:** Android (Developed in Android Studio)  
- **Languages Used:** Java and Kotlin  
- **Libraries & Dependencies:**
  - AndroidX Core, AppCompat, ConstraintLayout  
  - Material Design Components  
  - Navigation Components  
  - Biometric Library (for fingerprint scanning)  
  - ZXing (for QR code scanning)  
  - Retrofit + OkHttp + Gson (for REST API communication)  
  - Room Database (for local data storage)  
  - Lifecycle ViewModel + LiveData  
  - Kotlin Coroutines (for background tasks)  
  - Multidex, Annotations, Espresso & JUnit (for testing)  
- **Hardware Integration:** Mantra MFS100 Fingerprint Scanner  

---

### 🧰 Tools & Environment
- **IDE:** Visual Studio Code (Web), Android Studio (Mobile)  
- **Server Environment:** WAMP (Windows Apache MySQL PHP)  
- **Version Control:** Git & GitHub  
- **Email Service:** SMTP (used via Flask-Mail)  
- **Local Hosting:** PHP + Python on localhost  
- **Operating System:** Windows  

---

## 💡 Project Scope
- Developed as a **Postgraduate Final Year Project** (Solo Development).  
- All technologies learned and implemented through **self-study and online research**.  
- Demonstrates integration between **web systems, mobile applications, and biometric authentication**.

---

## 🚀 Future Improvements
- Add **WhatsApp or SMS alerts** for notifications.  
- Implement **AI-based hall allocation optimization** for large institutions.  
- Introduce **cloud-based backup** and data analytics dashboard for administrators.

---

## 🧑‍💻 Developer
- **Project Developer:** Maria Dorthy   
- **Institution:** Anna University 
- **Project Type:** PG Final Project (Solo)  
- Technologies learned and implemented independently with help from online resources.

---
## ⚖️ License
See [LICENSE.md](LICENSE.md) — All rights reserved.
