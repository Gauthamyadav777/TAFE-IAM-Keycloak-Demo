# TAFE Vocational LMS – Keycloak IAM Demo

Mock education-sector Identity & Access Management (IAM) system built to demonstrate SSO, RBAC, groups, user lifecycle and fine-grained authorisation.

<img width="709" height="360" alt="portal-before-login" src="https://github.com/user-attachments/assets/ba2f2c01-d6ad-4f72-a46a-5eb1a78f3911" />

## What This Project Demonstrates
- **Single Sign-On (SSO)** using OpenID Connect (Authorisation Code Flow)
- **Role-Based Access Control (RBAC)**: Students (view-only) vs Lecturers (full admin)
- **Groups** and **least privilege** principle
- **User lifecycle** simulation (onboard → assign group → access changes instantly)
- MFA-ready Keycloak configuration
- Education use-case: mirrors TAFE student/staff access patterns

## Technologies
- Keycloak 26.x (open-source IAM / alternative to Entra ID / AD)
- Docker
- Plain HTML + JavaScript (OIDC client flow)

## Quick Start (Local Demo)
1. Clone repo
2. Run: docker compose up
3. Open http://localhost:3000
4. Click "Login with TAFE IAM"
5. Test users:
- `demo-student` / `password123` → Student Dashboard
- `demo-lecturer` / `password123` → Lecturer Admin Dashboard

## Screenshots

### 1. Mock TAFE Portal (before login)
<img width="709" height="360" alt="portal-before-login" src="https://github.com/user-attachments/assets/2a40176e-cefa-488f-b5f6-603023b4e9fc" />


### 2. Keycloak Login Screen
<img width="777" height="545" alt="login-screen" src="https://github.com/user-attachments/assets/242e54e4-e027-48a5-a928-dc1500410a83" />

### 3. Student View (after login as demo-student)
<img width="937" height="639" alt="student-dashboard" src="https://github.com/user-attachments/assets/a95b3d34-b0e4-43ae-a035-e5ad85e9ad4b" />

### 4. Lecturer Admin View (after login as demo-lecturer)
<img width="807" height="582" alt="lecturer-dashboard" src="https://github.com/user-attachments/assets/eb090f6e-4b82-4702-8814-3a28d180ba92" />

### 5. Keycloak Admin – Realm Overview
<img width="1414" height="669" alt="realm-overview" src="https://github.com/user-attachments/assets/aec8e22f-e9ae-4c67-8a12-0a8dd905b78d" />

### 6. Groups Configuration
<img width="1418" height="670" alt="groups" src="https://github.com/user-attachments/assets/b50ffb49-3dd0-4334-9dc4-6613f97eb153" />

### 7. Logout Screen
<img width="974" height="564" alt="Log out screen" src="https://github.com/user-attachments/assets/21a4614c-1a37-45d3-8340-d17f99742f91" />

### 8. Docker Container
<img width="1262" height="564" alt="Docker container" src="https://github.com/user-attachments/assets/3e83117c-f534-49c8-85a7-3ff08a9e1742" />

### 9. Clients
<img width="1406" height="678" alt="clients" src="https://github.com/user-attachments/assets/1788f812-1e90-4425-b3ce-5b6be9cadc18" />

- **IDAM disciplines** (on-prem/cloud, SSO, MFA concepts)
- **Stakeholder communication** — simple UX for students/academics
- **Continuous improvement** — easy group/role changes
- **Incident support** — troubleshoot via admin console

Built by **Gautham Yadav** (Cert IV Cyber Security, Master's IT) as preparation for the Systems Engineer (IAM) position.

Feel free to fork/contact me for questions!
