# Construction Management System

A software-based concept for managing construction project information in one centralized system. The proposed system aims to make project records easier to maintain, search, update, and report compared with paper registers and separate spreadsheets.

> **Project status:** This documentation is based on the project presentation. It describes the proposed system and its requirements; it does not claim that the software has been implemented or tested. Update this section after adding your source code, screenshots, and verified implementation details.

## Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [Proposed Modules](#proposed-modules)
- [Users and Responsibilities](#users-and-responsibilities)
- [Functional Requirements](#functional-requirements)
- [Data Requirements](#data-requirements)
- [Feasibility Study](#feasibility-study)
- [System Diagrams](#system-diagrams)
- [Suggested Technology Stack](#suggested-technology-stack)
- [Future Enhancements](#future-enhancements)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Author](#author)

## Overview

Construction Management System is a proposed application for maintaining construction-related records digitally. The information covered includes projects, clients, workers, materials, suppliers, tasks, expenses, progress, and reports. A centralized database and user authentication are included in the proposed scope.

## Problem Statement

In the existing process described in the project presentation, records are often maintained through registers, paper files, and spreadsheets. This can make information slow to find or update and may lead to duplicated, misplaced, damaged, or inaccurate records. Manually tracking work progress, material availability, project budgets, and reports can also take time and make coordination difficult.

## Objectives

- Reduce dependence on manual paperwork.
- Keep construction records organized in one place.
- Make project, client, worker, material, and expense information easier to search and update.
- Support tracking of tasks and project progress.
- Maintain material and supplier records.
- Help record project budgets and expenses.
- Support timely report preparation.
- Restrict system access to authorized users through login credentials.

## Proposed Modules

| Module | Purpose |
|---|---|
| Project Management | Create, update, and monitor construction projects, including location and budget. |
| Client Management | Maintain client contact details and project requirements. |
| Worker Management | Maintain worker details, attendance, assigned tasks, job roles, and salary information. |
| Material Management | Record material purchases, quantities, stock availability, suppliers, and usage. |
| Expense Management | Record project expenses, dates, types, descriptions, and budget-related information. |
| Task Management | Maintain task descriptions, start/end dates, status, and assigned project/worker. |
| Progress Tracking | Record progress dates, percentages, descriptions, and status. |
| Supplier Management | Maintain supplier contact details and the materials supplied. |
| Reports | Store report metadata and support report preparation. |
| User Authentication | Allow authorized users to sign in using login credentials. |

## Users and Responsibilities

- **Project Manager:** manages projects, schedules work, and monitors progress and activities.
- **Site Engineer:** updates site progress and technical information.
- **Contractor:** coordinates workers, assigned tasks, and construction activities.
- **Material Manager:** maintains purchase, stock, and material-usage records.
- **Accountant:** maintains expense, budget, payment, and financial records.
- **Administrator:** manages system users, records, and general system operations.

## Functional Requirements

The proposed system should allow authorized users to:

1. Create and update project records.
2. Maintain client information.
3. Add and maintain worker records and attendance.
4. Record construction materials, quantities, suppliers, and usage.
5. Record supplier information.
6. Create tasks and associate them with projects and workers.
7. Record progress updates, percentage completion, and status.
8. Record expenses with type, amount, date, and description.
9. Prepare or maintain project-related reports.
10. Authenticate users and limit access to authorized users.

## Data Requirements

The presentation identifies the following data fields as requirements. These are proposed fields, not a confirmed implemented database schema.

| Entity | Example fields |
|---|---|
| User | User ID, name, username, password, email |
| Project | Project ID, project name, description, client name, location, budget |
| Client | Client ID, name, address, contact number, email |
| Material | Material ID, name, quantity, unit, supplier name |
| Worker / Employee | Worker ID, name, contact number, address, job role, salary |
| Task | Task ID, name, description, start date, end date, status, project ID, worker ID |
| Supplier | Supplier ID, name, contact number, address, email, material supplied |
| Progress | Progress ID, project ID, progress date, progress percentage, description, status |
| Expense | Expense ID, project ID, expense type, amount, expense date, description |
| Report | Report ID, project ID, report type, report date, description, generated by |

**Security note:** passwords should never be stored as plain text in a real implementation. Use a suitable password-hashing mechanism and apply role-based authorization and secure database practices.

## Feasibility Study

### Technical feasibility
The presentation suggests common web technologies such as HTML, CSS, JavaScript, PHP/Python/Java, and MySQL as possible implementation choices. A typical computer and database software may be sufficient for a basic implementation.

### Economic feasibility
The proposed system may reduce paper use and time spent maintaining and searching records. Actual development and maintenance costs depend on the final technology choices and deployment requirements.

### Operational feasibility
The system is intended to be straightforward for project managers and authorized staff to use for maintaining projects, workers, materials, expenses, and reports. Usability should be confirmed through testing with intended users.

## System Diagrams

The presentation lists these system-design diagrams:

- E-R Diagram
- Class Diagram
- Object Diagram
- Component Diagram
- Deployment Diagram
- Use Case Diagram
- Activity Diagram
- State Chart Diagram
- Sequence Diagram
- Collaboration Diagram

Add the actual diagram images or source files to a `docs/diagrams/` directory and link them here. The presentation's diagram slides should be checked to ensure each diagram is visible and readable before publishing.

## Suggested Technology Stack

The presentation lists these as possible technologies, not a confirmed final stack:

- **Front end:** HTML, CSS, JavaScript
- **Back end:** choose one—PHP, Python, or Java
- **Database:** MySQL

Update this section to match the technologies actually used in your code. Avoid listing multiple alternatives as if all are implemented.

## Future Enhancements

Potential future improvements, subject to project scope, include:

- Dashboard showing project status and key summaries.
- Search, filtering, and export options for reports.
- Notifications for task deadlines and low material stock.
- Role-based access permissions.
- Backup and restore facilities.
- Responsive interface for phones and tablets.

## Getting Started

This repository currently contains project documentation. Once source code is added, replace this section with the exact setup steps for the chosen technology stack. A useful setup guide should state prerequisites, database creation/import steps, configuration values, how to run the application, and how to use demo/test credentials if applicable. Do not publish real passwords, API keys, or private data.

## Project Structure

Suggested repository layout:

```text
construction-management-system/
├── README.md
├── docs/
│   ├── Project_Documentation.docx
│   └── diagrams/
├── src/                  # Add application source code here, if available
├── database/             # Add schema or sample SQL here, if available
└── screenshots/          # Add genuine application screenshots here
```

## Author

- **Name:** Add your name
- **Course / Department:** Add your course and department
- **Institution:** Add your college/institution
- **Project:** Construction Management System

## Important before publishing

1. Replace author placeholders with your details.
2. Add source code only if you have it and can explain it.
3. Add genuine screenshots and the actual diagrams.
4. Update the technology stack and setup instructions to match the implementation.
5. Do not claim deployment, testing, or completed features unless you have verified them.
