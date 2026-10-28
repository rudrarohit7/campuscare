# CampusEvent – College Event Management & Digital QR Pass System

> **A modern, centralized campus event management, digital ticket issuance, and high-speed QR attendance verification platform built with ASP.NET Core MVC 8, Entity Framework Core 8, MySQL, and QuestPDF.**

---

## 🌟 Key Features

### 🎓 1. Public & Student Self-Service Portal
- **Centralized Event Discovery**: Real-time event catalog with instant category filtering (Hackathon, Technical, Cultural, Sports, Workshop, Seminar) and search.
- **Live Seat Availability Tracking**: Dynamic seat capacity counters with real-time registration status.
- **Student Account Onboarding**: Integrated registration capturing student academic profile (Enrollment ID, Department, Course, Semester).
- **Personal Passes Hub**: Student dashboard to view booking history, access active event passes, and re-download PDF tickets.
- **Dual Pass Formats**: Instant interactive Web Pass with dynamic QR code and downloadable 61 KB vector PDF ticket.

### 🎟️ 2. Digital QR Passes & QuestPDF Engine
- **Vector PDF Ticket Generation**: On-the-fly compilation of high-resolution vector PDF tickets via QuestPDF engine upon registration.
- **Anti-Fraud Security**: Unique GUID vector tokens embedded in QR codes to prevent pass forgery and ticket duplication.
- **Automated SMTP Email Delivery**: Registration confirmation emails with event guidelines and the vector PDF pass attached directly via MailKit.

### 📷 3. Coordinator Hub & Live Camera Scanner
- **Zero-File-Upload Camera Scanning**: Browser-based live camera stream scanning powered by HTML5-QRCode directly on mobile/laptop webcams.
- **Instant Gate Verification Modal**: Audible chime feedback and real-time pop-up modal displaying verified attendee name, photo, enrollment number, and event details.
- **Strict Anti-Fraud Protection**: Relational database constraints immediately flag and reject duplicate pass scans.
- **Venue Attendance Roster**: Real-time check-in log providing coordinators with live gate turnout metrics.

### 🛡️ 4. Administrator Command Center
- **Executive KPI Dashboard**: Live monitoring of total events, active registrations, gate attendance rates, and recent activity.
- **Comprehensive Event Management**: Full CRUD operations to create events, configure registration cut-offs, allocate seat quotas, and toggle visibility.
- **Staff & Coordinator Assignments**: Dedicated console to assign faculty and student coordinators to specific campus events.
- **Academic Hierarchy Management**: Structured mapping of University Departments (e.g., Computer Science, IT) and Academic Courses (e.g., B.Tech CSE, MCA).
- **Attendee & Attendance Audits**: Filterable reports of student registrations, verified attendance timestamps, and verifying coordinators.
- **User Directory & Security**: Role-Based Access Control (RBAC) managing Admin, Coordinator, and Student accounts with status toggles.
- **SMTP Audit Logs**: Delivery logs tracking outgoing confirmation emails and attachment statuses.

---

## 📸 Screenshots & Output Showcase

### 1. Public & Student Portal

#### 1.1 Home Page – Hero Section
Displays university branding, headline, event registration call-to-action, and pass preview.
![Home Page Hero](wwwroot/images/screenshots/01_home_hero.png)

---

#### 1.2 Home Page – Events Catalog, Stats & Dark Footer
Campus metrics cards, upcoming events showcase with category badges, and institutional contact footer.
![Home Events & Footer](wwwroot/images/screenshots/02_home_events_and_footer.png)

---

#### 1.3 Available Events Catalog & Search
Complete event catalog with category filtering (Hackathon, Tech, Cultural, Sports), keyword search, and live seat counters.
![Events Catalog](wwwroot/images/screenshots/03_events_catalog.png)

---

#### 1.4 Event Details & Registration Screen
Event schedule, venue details, coordinator contact info, and registration submission form.
![Event Details](wwwroot/images/screenshots/04_event_details.png)

---

#### 1.5 Student Registration & Account Sign-Up
Student onboarding form capturing Enrollment ID, Department, Course, Semester, Mobile Number, and Password.
![Student Registration](wwwroot/images/screenshots/05_student_register.png)

---

#### 1.6 Student Login Page
Secure authentication gateway for students to manage bookings and download event passes.
![Student Login](wwwroot/images/screenshots/06_student_login.png)

---

#### 1.7 Student My Registrations & Passes Hub
Personal attendee portal listing all booked events, check-in statuses, and pass download links.
![Student Passes](wwwroot/images/screenshots/07_student_passes.png)

---

#### 1.8 Official Digital Event Pass (Web View)
Interactive digital event badge displaying student name, enrollment number, venue details, and anti-fraud QR code.
![Digital Event Pass](wwwroot/images/screenshots/08_digital_event_pass.png)

---

#### 1.9 Downloaded Vector PDF Event Pass (QuestPDF Engine)
Clean, high-resolution vector PDF ticket dynamically compiled with student badge, QR code, and venue guidelines.
![PDF Pass Document](wwwroot/images/screenshots/09_pdf_pass_download.png)

---

#### 1.10 Automated Registration Confirmation Email with Attached PDF Pass
Automated email notification delivering event details, entry instructions, and the attached vector PDF pass.
![Email with Attached PDF Pass](wwwroot/images/screenshots/10_email_with_pdf_pass.png)

---

### 2. Administrator Portal & Operations

#### 2.1 Staff & Admin Login
Dedicated authentication gateway for campus administrators and event coordinators.
![Admin Login](wwwroot/images/screenshots/11_admin_login.png)

---

#### 2.2 Administrator Command Dashboard
Overview console displaying real-time metrics, quick operational shortcuts, and recent registration activity feed.
![Admin Dashboard](wwwroot/images/screenshots/12_admin_dashboard.png)

---

#### 2.3 Event Management Console
Event administration table displaying category tags, dates, venues, seat capacity ratios, and edit/delete actions.
![Admin Manage Events](wwwroot/images/screenshots/13_admin_manage_events.png)

---

#### 2.4 Create New Event Form
Event creation console to configure title, category, description, date/time, venue, seat quota, fee, and banner image.
![Admin Create Event](wwwroot/images/screenshots/14_admin_create_event.png)

---

#### 2.5 Coordinators Management & Event Assignment
Management panel to register event coordinators and assign them to oversee specific campus events.
![Admin Coordinators](wwwroot/images/screenshots/15_admin_coordinators.png)

---

#### 2.6 Academic Departments & Courses Hierarchy
Academic administration view to configure University Departments and associate specific Academic Courses.
![Admin Academic](wwwroot/images/screenshots/16_admin_academic.png)

---

#### 2.7 Registrations List & Attendee Audit
Complete attendee roster listing registered student names, enrollment IDs, departments, event titles, and verification tokens.
![Admin Registrations](wwwroot/images/screenshots/17_admin_registrations.png)

---

#### 2.8 Campus Attendance Report
Gate check-in audit report with verified student details, verifying coordinator names, and check-in timestamps.
![Admin Attendance](wwwroot/images/screenshots/18_admin_attendance.png)

---

#### 2.9 User Accounts Directory
User administration table displaying all registered users, assigned roles (Admin, Coordinator, Student), and status toggles.
![Admin Users](wwwroot/images/screenshots/19_admin_users.png)

---

#### 2.10 SMTP Email Delivery Logs
Comprehensive audit trail of outgoing confirmation emails, recipient addresses, pass attachment statuses, and timestamps.
![Admin Email Logs](wwwroot/images/screenshots/20_admin_email_logs.png)

---

### 3. Coordinator Hub & Verification Desk

#### 3.1 Coordinator Dashboard
Dashboard for event coordinators displaying assigned events, registered attendee counts, and one-click scanner launch.
![Coordinator Dashboard](wwwroot/images/screenshots/21_coordinator_dashboard.png)

---

#### 3.2 Live Camera QR Scanner (Viewfinder & Sound Toggle)
Sub-second camera scanner using HTML5-QRCode with audio beep toggle and real-time scan feed.
![Coordinator Scanner](wwwroot/images/screenshots/22_coordinator_scanner.png)

---

#### 3.3 Instant Verification Pop-up Modal
Real-time modal pop-up displaying verified attendee profile, full name, enrollment number, and check-in confirmation.
![Coordinator Modal Popup](wwwroot/images/screenshots/23_coordinator_scan_modal.png)

---

#### 3.4 Coordinator Attendance Roster
Live check-in roster for coordinators to track verified attendees present at the venue.
![Coordinator Attendance Roster](wwwroot/images/screenshots/24_coordinator_attendance_roster.png)

---

### 4. User Profile & Settings

#### 4.1 Profile & Security Settings
Profile console allowing staff and coordinators to update profile information and security credentials.
![Account Profile Dashboard](wwwroot/images/screenshots/25_account_profile_dashboard.png)
