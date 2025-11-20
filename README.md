# ICT171-Cloud-Server-Project
Farhaan Torgal - To-Do List Website hosted on Azure VM, using domain from godaddy.
# ICT171 Cloud Server Project — To-Do List Web App

**Student Name:** Farhaan Torgal  
**Student Number:** 35806405 
**Unit:** ICT171 – Introduction to Cloud Computing  
**Institution:** Murdoch University  

---

## 1. Project Overview

This project implements a simple **To-Do List web application** hosted on a **Microsoft Azure Ubuntu Virtual Machine (IaaS)** and exposed publicly through a custom domain with **HTTPS** enabled.

The goal of the project is to demonstrate that I can:

- Provision and manage an **IaaS virtual machine** in Azure  
- Install and configure a **web server (Nginx)**  
- Deploy a **custom website** (HTML/CSS/JavaScript)  
- Configure **DNS** so the site is reachable via a domain name  
- Secure the site using **Let’s Encrypt TLS certificates (HTTPS)**  
- Document how to rebuild the environment

---

## 2. Live Server Details

**Domain Name:**  
- https://farhaantodolist.online  
- https://www.farhaantodolist.online  

**Public IP Address (Azure VM):**  
- `20.233.250.135`

**Cloud Provider:**  
- Microsoft Azure

**VM Type:**  
- Ubuntu Linux VM (IaaS)  
- Web server: **Nginx**

---

## 3. Application Description

The deployed application is a **simple To-Do List web app** that allows the user to:

- Add new tasks  
- Mark tasks as completed  
- Edit existing tasks  
- Delete tasks  
- Filter tasks by **All / Active / Completed**  
- Persist tasks in the browser using **localStorage**  

The stack is **pure front-end**:

- `index.html` — structure and layout  
- `styles.css` — dark-themed responsive styling  
- `app.js` — JavaScript logic for task management and localStorage  

No server-side code is required beyond Nginx serving static files.

---

## 4. Repository Structure

```text
ICT171-Cloud-Server-Project/
├─ index.html          # To-Do List HTML
├─ styles.css          # Styling (dark theme)
├─ app.js              # JavaScript logic, localStorage, filters, edit/delete
├─ scripts/
│   └─ backup_todo.sh  # Simple backup script for /var/www/todo
└─ README.md           # This documentation
