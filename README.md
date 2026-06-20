# AFS — Assessment Feedback System (Java)

A Java desktop application simulating a role-based academic assessment and feedback system, built for an Object-Oriented Development with Java module. The system supports four distinct user types — Admin Staff, Academic Leader, Lecturer, and Student — each with their own dashboard and permissions.

## Overview

AFS runs as a single local desktop application — no networking, no multi-user concurrency, no database. All data is read from and written to plain text (`.txt`) files, as required by the module's scope. The focus of the project is applying core object-oriented principles to model real-world entities (users, courses, assessments, results, feedback) cleanly through classes and their relationships.

## User Roles & Features

**Admin Staff**
- Create, update, and delete user accounts
- Assign lecturers to academic leaders
- Configure the grading system (score ranges per grade)
- Create and manage classes

**Academic Leader**
- Create, update, and delete modules
- Assign lecturers to modules
- View analyzed reports
- View lecturer and student feedback

**Lecturer**
- Design assessments
- Key in student marks
- Provide feedback

**Student**
- Register for classes
- Check results
- Provide feedback

All roles can log in and edit their own profile.

## OOP Concepts Applied

- **Abstraction** — `User` implemented as an abstract class
- **Encapsulation** — private fields accessed through getters/setters
- **Inheritance** — `User` as the superclass, with role-specific subclasses (e.g. `AdminStaff`)
- **Polymorphism** — method overriding for user identification across roles
- **Modularity** — package-level organization by role

## Tech Stack

- Java (`java.awt` / `java.swing` for the GUI)
- Plain text (`.txt`) file storage — no database

## Limitations

- Single-user local desktop app — no networking or concurrent multi-user support
- Plain-text storage rather than a real database
- Basic authentication only, no advanced security hardening

## Module

Built for CT038-3-2-OODJ (Object Oriented Development with Java) — Group 8 (Lab-64).

## Team

- **Hafiy Ziyad Zikry** — Group Leader, Admin Staff module
- **Lutfil Hadi** — Academic Leader module
- **Mohd Afif Ammarhazim** — Lecturer module
- **Iddin Irfan Mikhail** — Student module
