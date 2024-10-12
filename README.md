# careForceOne
# CareForceOne

CareForceOne is a comprehensive healthcare staffing and management SaaS solution, built to streamline healthcare workflows, documentation, and patient care. This solution provides features for nurses, healthcare providers, and clinics, including AI-assisted documentation, applicant tracking, smart scheduling, and more.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Architecture Overview](#architecture-overview)
- [Modules](#modules)
- [License](#license)

## Introduction

CareForceOne offers a powerful set of tools to improve the day-to-day management of healthcare services. From **nurses notes** to **care plans** and **smart scheduling**, CareForceOne provides an end-to-end solution that saves time, reduces paperwork, and enhances care quality.

CareForceOne is built with **Directus** for data management and **Node.js** for custom API development. CareForceOne is containerized using **Docker** for easy deployment and scalability.

## Features

- **Nurses Notes**: Streamlined, AI-assisted notes that save time on documentation, allowing nurses to focus more on patient care.
- **Applicant Tracking System (ATS)**: Manage and track applicants easily with an integrated ATS.
- **Smart Scheduling**: Automate the process of scheduling visits and replacing staff due to last-minute cancellations.
- **Customizable Templates**: User-defined note templates for multiple domains (e.g., healthcare, veterinary) to ensure flexibility.
- **AI Auto-Completion**: AI-driven auto-completion of clinical notes with user approval, modification, or retry options.
- **Role-Based Access**: Define roles and manage permissions for users, ensuring secure data access.

## Getting Started

These instructions will help you set up CareForceOne on your local machine for development and testing purposes.

### Prerequisites

- **Docker** and **Docker Compose**
- **Node.js** and **npm**
- **PostgreSQL**

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/careforceone.git
   cd careforceone
   ```

2. **Environment Variables**:
   - Create a `.env` file at the root directory and add the required environment variables, such as database credentials, API keys, and Directus configurations.

3. **Run Docker Containers**:
   ```bash
   docker-compose up --build
   ```

4. **Initialize the Database**:
   Run the database migration and seed commands to set up the PostgreSQL database.

5. **Start the Backend Server**:
   ```bash
   npm install
   npm run start
   ```

## Usage

Once everything is up and running, you can access the CareForceOne backend APIs via **http://localhost:3000**. The **Directus CMS** will be available at **http://localhost:8055**.

For documentation generation, AI-powered note completion, and other advanced features, ensure that the appropriate environment variables and APIs are properly configured.

## Architecture Overview

CareForceOne follows a **microservice architecture** using **Docker** and **Kubernetes** for scalability.

- **Directus CMS**: Manages data storage, roles, and permissions for the app.
- **Node.js**: Custom APIs, logic for AI completions, and tenant management.
- **PostgreSQL**: Database for storing patients, providers, notes, applicants, etc.
- **Docker and Kubernetes**: Containerization for scalability and deployment.

## Modules

1. **Applicant Tracking System**
2. **Job Board Platform**
3. **Applicants Management**
4. **Patients**
5. **Providers**
6. **Nurses Notes** (AI-driven)
7. **Leads / Referrals**
8. **Smart Scheduling**
9. **Visits / Verification**
10. **Care Plans**
11. **Timesheets / Approvals**
12. **Clients / Facilities**
13. **EHR Integration**
14. **Dashboard**
15. **Reporting**
16. **System Administration**

## License

CareForceOne is a proprietary software solution. All rights reserved. For licensing information, please contact us directly.
