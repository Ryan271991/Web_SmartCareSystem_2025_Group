# Smart Care System 🏥
<img width="946" height="545" alt="image" src="https://github.com/user-attachments/assets/f69b3bde-f0a2-4b8e-83d2-b4d97181871a" />

An appointment and patient record management system for medical clinics, designed to relieve administrative burdens and improve patient care.

---

## 🌟 Core Features

* **Account Management:** Secure registration, login, and Role-based Access Control for different users (Patient, Doctor, Receptionist).
* **Smart Booking:** Allows precise appointment scheduling with a mechanism to prevent double booking using Prisma transactions.
* **Schedule Management:** Displays available doctors, and allows flexible management and updating of appointment statuses (canceling or rescheduling).
* **Medical Records:** Provides features to look up patient history, view past visits, and add diagnosis notes exclusively for doctors.
* **Statistics & Reports:** Features a statistical dashboard and generates daily activity reports for the clinic.

## 💻 Tech Stack

* **Frontend:** React.js, CSS.
* **Backend:** Node.js.
* **Database:** SQL with Prisma ORM.
* **Authentication:** Role-based Access Control using JSON Web Tokens.

## 🧪 Testing System

The project implements an in-depth software testing process to ensure quality, focusing specifically on the Doctor's Availability feature:

* **Black Box Testing:** Applies Equivalence Partitioning and Boundary Value Analysis techniques to the limits of date, time, and doctor selection inputs.
* **White Box Testing:** Achieves 100% Branch Coverage and Statement Coverage for data retrieval processing flows.
* **Unit Testing:** Uses the Jest framework to test controllers. The system integrates mocking techniques to create fake versions of the database model, allowing tests for success and error scenarios (500 Server error, 400 Bad request) without affecting real data.

## 🚀 Installation & Setup

**1. Prerequisites:**

Ensure you have Node.js installed on your machine.

**2. Clone the repository:**

```bash
git clone [https://github.com/Andrewsemafumu/Team-Project-](https://github.com/Andrewsemafumu/Team-Project-)
```
**3. Run the Server (Frontend & Backend):**
Navigate to the backend and frontend directories (installation packages are pre-zipped, so no install command is needed), then execute the following command:

```bash
npm run dev
```
**4. Database Setup:**
Open a terminal in the backend directory and run the following Prisma commands in order to generate and run the database on localhost:


```bash
npx prisma generate
npx prisma migrate dev
npx prisma studio
```

## 👥 Team Members (Team 8)
* **Le Hoang Huynh:** Set up the login/access system, managed appointment rescheduling, built the patient medical history lookup, handled appointment status tracking, and developed the entire Testing process.
* **Timothy Semafumu:** Managed doctor availability, optimized application load times, and ensured the security of patient records.
* **Kamlesh Choudhary:** Built the new patient registration, online appointment booking, and daily report generation features.
* **Enrico Frossard:** Designed the statistics dashboard, developed diagnosis notes, and implemented the database logic to prevent double booking


