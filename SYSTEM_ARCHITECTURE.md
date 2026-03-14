# AfriNuts Farm OS – System Architecture

## Overview

AfriNuts Farm OS is an Android application designed to manage farm operations for AfriNuts Export.

The system follows a layered architecture.

---

## Technology Stack

Frontend:
Android (Java)

UI Framework:
Material Design Components

Local Database:
Room Database (SQLite)

Cloud Synchronization:
Firebase

Architecture Pattern:
MVVM (Model View ViewModel)

---

## Core Modules

### Farm Module

Handles:

• Farm creation
• Farm information
• Farm settings

---

### Block Management

Tracks farm blocks.

Each block contains:

• Block name
• Status
• Harvest data

---

### Revenue Module

Records harvest income.

Fields include:

• Quantity
• Price per kg
• Harvest date
• Quality grade
• Buyer

---

### Expense Module

Tracks farm costs.

Examples:

• Labor
• Equipment
• Transport

---

### Task Management

Allows managers to assign tasks to workers.

Tasks contain:

• Title
• Assigned worker
• Due date
• Status

---

## Data Storage

### Local Storage

Room database tables:

• farms
• blocks
• revenue
• expenses
• tasks

---

### Cloud Sync

Firebase synchronization ensures that:

• Data is backed up
• Multiple devices stay updated

---

## Security

Authentication controls access based on roles:

• Owner
• Manager
• Worker

Sensitive financial data is restricted to authorized users.

---

## Future Improvements

Planned upgrades include:

• Offline-first synchronization
• Blockchain traceability for harvest batches
• Processing center integration
• Advanced analytics
