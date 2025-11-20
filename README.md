# COP4331 Team 10 – Contact Manager (LAMP Stack)

Contact manager web application built as the **small project** for  
**COP 4331C – Processes for Object-Oriented Software Development** at UCF.

The app lets users register, log in, and manage a personal address book of contacts
(create, search, update, delete) using a classic LAMP stack (Linux, Apache, MySQL, PHP)
with an HTML/CSS/JavaScript frontend.

> **Your Role (Minh Thien Pham)**  
> I implemented the PHP backend APIs in `/LAMPAPI`  
> (**Login, Register, AddContact, UpdateContact, DeleteContact, SearchContacts**).  
> You can view that code here:  
> 👉 [`/LAMPAPI` folder](https://github.com/MinhThien-Pham/COP4331-Team10-Project1/tree/main/LAMPAPI)

> This repository is a **fork** of the original team project by  
> Jackson Cammack and teammates, maintained here by **Minh Thien Pham**
> to document the project and personal API contributions.

---

## Project Overview

- **Course**: COP 4331C – Processes for Object-Oriented Software Development (UCF)
- **Type**: Team project (small web app)
- **Role (this fork)**: Backend API developer for the `LAMPAPI` PHP endpoints
- **Original upstream**: https://github.com/JacksonCammack-UCF/COP4331-Team10-Project1
- **This fork**: https://github.com/MinhThien-Pham/COP4331-Team10-Project1

### Features

- User registration and login
- Session-based personal contact list
- Create / read / update / delete (CRUD) contacts
- Search contacts by text (name, email, etc.)
- Pre-built schema and seed data for quick setup

---

## Tech Stack

**Frontend**

- HTML5 (landing, login, contacts, register pages)
- CSS3 for layout and styling
- Vanilla JavaScript for form handling and API calls (`/js`)

**Backend**

- PHP 7+ (procedural LAMP-style API in `/LAMPAPI`)
- MySQL database (schema + seed data in `schema.sql` and `seed.sql`)
- Apache (or any server that can run PHP)

---

## API Documentation (Swagger)

This project includes an OpenAPI/Swagger specification for the PHP LAMP APIs
(Login, Register, AddContact, SearchContacts, UpdateContact, DeleteContact).

- Swagger file: [`docs/swagger.yaml`](./docs/swagger.yaml)

---

## Project Structure

```text
.
├── LAMPAPI/          # PHP endpoints
│   ├── AddContact.php
│   ├── DeleteContact.php
│   ├── Login.php
│   ├── Register.php
│   ├── SearchContacts.php
│   └── UpdateContact.php
├── css/              # Stylesheets
├── images/           # UI images / assets
├── js/               # Frontend JavaScript (API calls, DOM updates)
└──docs/
│   └── swagger.yaml  
├── contacts.html     # Contacts UI (CRUD + search)
├── index.html        # Landing / login page
├── register.html     # Registration page
├── schema.sql        # Database schema (tables, indexes)
└── seed.sql          # Sample data for quick testing
