# MediCall: Secure Teleconsultation Platform

## 1. Project Overview

**MediCall** is a comprehensive software solution developed as a **Final Year Project (FYP)** for the Bachelor's degree. It establishes a secure, web-based platform designed to **efficiently manage medical practices and patient appointments**. The core objective is to leverage digital technology to enhance the administrative workflow, scheduling, and patient record management within primary healthcare centers.

### 1.1 Problem Context

The primary challenge identified is the need for an innovative solution for the efficient management of medical practices. While numerous software solutions exist for managing clinics, they often feature complex and poorly ergonomic interfaces that do not consistently meet the specific needs of healthcare professionals.

In this context, our objective is to design and implement a user-friendly and intuitive web application with advanced features. We aim to simplify the daily routines of healthcare professionals by providing a platform that is easy to use and tailored to their specific needs. This will allow them to save time and focus on their primary mission: patient care.

### 1.2 Key Objectives

* To design and implement dedicated, feature-rich interfaces for both the Doctor and the Patient, prioritizing *ergonomics* and *intuitiveness*.
* To provide robust scheduling and calendar management for practitioners.
* To develop a secure system for patient registration, authentication, and medical record management.
* To ensure compliance with data protection standards (e.g., GDPR, HIPAA - *Mention the relevant standard for your region*).
* To provide an intuitive and responsive user experience across devices.

## 2. Technical Architecture

MediCall adopts a modern, decoupled architecture to ensure scalability, maintainability, and specialized performance.

### 2.1 Technology Stack

| Component | Technology | Role |
| :--- | :--- | :--- |
| **Frontend** | **React** | Client-side interface development and state management. |
| **Backend** | **Node.js (Express)** | RESTful API server, business logic, and security middleware. |
| **Database** | **MongoDB** | Persistent storage for application and patient data. |
| **Authentication** | **JWT** | Secure user identification and access control (Login/Signup). |

## 3. Core Functionalities

The application implements distinct interfaces for the patient and the physician, accessible via a mandatory authentication layer (Login/Signup).

### 3.1 Doctor Interface Features

The Doctor Interface is designed for fluid and efficient daily clinical practice, featuring a top navigation bar and a left-hand Sidebar for easy navigation.

| Sidebar Item | Description |
| :--- | :--- |
| **Dashboard** | Provides vital statistics (daily patient count), an upcoming appointment calendar view, and a task list for work organization. |
| **Agenda** | Full-screen calendar view for comprehensive schedule management, allowing the doctor to add events, check availability, and plan new appointments. |
| **Patients** | Management and viewing of the doctor's patient list, with the ability to add new patients and enter relevant information. |
| **Appointments** | Overview of all scheduled appointments. Doctors can add new appointments, specifying dates, times, and relevant details. |
| **Consultations** | Management of past consultations. Allows the doctor to add new consultation records, save important information, and access the history of prior consultations. |
| **Settings** | Personalization options, including profile updates, notification management, and other preference configurations. |

### 3.2 Patient Interface Features

The Patient Interface is designed to simplify appointment booking and personal medical record management.

* **Doctor Search:** Patients can search for available doctors using various criteria, such as specialty or location.
* **Appointment Booking:** Once a doctor is selected, the patient can choose a date and time to book an appointment. A confirmation is received after validation.
* **Medical Record Management:** Patients can scan and upload medical documents to enrich their file. This information is accessible to the doctor during consultations.
* **Favorites Management:** Patients can add doctors to a favorites list for quick access to their information and streamlined re-booking.

## 4. Getting Started

These instructions will guide you through setting up a copy of the project on your local machine for development and testing purposes.

### 4.1 Authentication

The application requires users to authenticate. Access is granted via the **Login page** or by creating a new account on the **Signup page**.

### 4.2 Prerequisites

Ensure you have the following software installed:

* Git
* [e.g., Node.js (v16+)]
* [e.g., Python (v3.9+)]
* [e.g., npm or Yarn]

### 4.3 Installation Steps

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/lotfi8rbh/MediCall.git](https://github.com/lotfi8rbh/MediCall.git)
    cd MediCall
    ```

2.  **Backend Setup**
    ```bash
    cd backend/
    # Install dependencies
    npm install  # or pip install -r requirements.txt
    
    # Create and configure the environment file
    cp .env.example .env
    # NOTE: Update the .env file with your database and API keys.
    
    # Start the server
    npm start # or python app.py
    ```

3.  **Frontend Setup**
    ```bash
    cd ../frontend/
    # Install dependencies
    npm install
    
    # Create and configure the environment file
    cp .env.example .env
    # NOTE: Update the .env file with the Backend API URL.
    
    # Start the application
    npm run dev
    ```

The application will be accessible in your browser at: `http://localhost:[PORT]` (e.g., `http://localhost:3000`).

## 5. Project Authorship

**[Your First Name Last Name]**
* **GitHub Profile**: [@lotfi8rbh](https://github.com/lotfi8rbh)
* **LinkedIn Profile**: [Link to your professional LinkedIn]
* **Email**: [Your academic or professional email address]

## 6. License

This project is licensed under the **[Ex: MIT / Apache 2.0 / etc.] License**. See the `LICENSE` file for details.
