# Procurement Order Tracking System (POTS)

This repository contains the source code and data files for a **Java-based Procurement Order Tracking System (POTS)** developed as part of a group assignment for the **Object Oriented Development with Java (CT038-3-2-OODJ)** module at Asia Pacific University.

## ❗Overview

**POTS** is a menu-driven Java application that automates and streamlines the procurement workflow for **Nexus Sdn Bhd (NSB)**, a growing wholesaler based in Kuala Lumpur. The system handles the full lifecycle of purchasing, from requisition by Sales Managers to approval and payment by Finance, using structured roles and object-oriented programming techniques.  

This project emphasizes:
- Effective use of OOP principles (inheritance, encapsulation, polymorphism, abstraction)
- Role-based access control
- File-based data management
- Modular and maintainable code structure

## User Roles & Access Rights

| Role | Key Functionalities |
|------|---------------------|
| **Administrator** | Register users (SM, PM, IM, FM, Admin), full access to system |
| **Sales Manager (SM)** | View items & stock, add daily sales, create/view purchase requisitions, view purchase orders |
| **Purchase Manager (PM)** | View requisitions, generate/edit/delete purchase orders, view suppliers & items |
| **Inventory Manager (IM)** | Add/edit/delete items & suppliers, update stock after delivery |
| **Finance Manager (FM)** | Approve/reject POs, process payments, track supplier payments, view stock status |

## Features

### Login System
- Secure login with validation
- Role-based access with individual user IDs
- User data stored in `users.txt`

### Item & Supplier Management
- Add/edit/delete items and suppliers
- Prevent duplicate entries
- Items linked to registered suppliers only

### Daily Sales Entry
- Sales Managers can record daily item-wise sales
- Sales affect stock levels

### Purchase Requisition (PR)
- SMs can create PRs with item code, quantity, due date
- System fetches linked supplier
- Each PR has a unique ID and is tracked

### Purchase Order (PO)
- POs generated only by PMs from approved PRs
- Includes tracking of the PM and supplier
- Viewable list of all POs by authorized roles

### Finance Operations
- FMs verify stock updates and approve/reject POs
- Payment processing and supplier payment tracking

## Data Storage

- All data (users, items, suppliers, PRs, POs) is saved in text files
- Easy to back up and migrate
- Ensures portability and simplicity for evaluation

## ❓How to Compile & Run

1. Download the full project ZIP file.
2. Open the folder in any Java IDE (e.g., NetBeans).
3. Compile and run the folder `Final`.
4. Follow the terminal-based menu options to navigate.

