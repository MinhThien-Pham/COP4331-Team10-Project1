# COP4331 Team 10 – LAMPAPI Backend (Contact Manager API)

This folder contains the **PHP backend APIs** for the Team 10 Contact Manager web application, built as the small project for:

> **Course**: COP 4331C – Processes for Object-Oriented Software Development (UCF)

The APIs here power user authentication and full contact CRUD (create, search, update, delete) for the frontend pages in the main project.

> **Maintainer of this folder**: **Minh Thien Pham**  
> Role: Implemented and maintained the PHP API endpoints in `LAMPAPI`.

> API docs: See the Swagger/OpenAPI spec at
> [`../docs/swagger.yaml`](../docs/swagger.yaml).

---

## Overview

The Contact Manager app lets users:

- Register a new account
- Log in with their credentials
- Manage a **personal** list of contacts:
  - Add new contacts
  - Edit existing contacts
  - Delete contacts
  - Search their contacts

All of those actions go through the PHP scripts in this `LAMPAPI` folder.

---

## Tech Stack

- **Language**: PHP 7+
- **Database**: MySQL / MariaDB
- **Architecture**: Classic LAMP-style JSON APIs
- **Data format**: JSON request + JSON response
- **Client**: HTML/CSS/JavaScript frontend in the root project

---

## Files in This Folder

Typical structure:

```text
LAMPAPI/
├── AddContact.php
├── DeleteContact.php
├── Login.php
├── Register.php
├── SearchContacts.php
└── UpdateContact.php
