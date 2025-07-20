# PHP Form + MySQL Data Table with Status Toggle

This is a simple yet functional full-stack web application that demonstrates how to collect user input through a form, store it in a MySQL database, display the stored data, and interact with it dynamically.

## 🛠️ Features

- One-line form to submit:
  - Name
  - Age
- Data is inserted into a MySQL database via PHP.
- Records are displayed in a styled HTML table.
- Each record has a toggle button to switch `status` between `0` and `1`.
- Toggling the status updates the database instantly using AJAX (JavaScript + PHP).
- Status updates are reflected immediately on the webpage without reload.

## 💻 Technologies Used

- **HTML** – For page structure and form.
- **CSS** – For basic styling.
- **JavaScript (Fetch API)** – For handling the status toggle without page reload.
- **PHP** – Backend logic for inserting and updating data.
- **MySQL** – Data storage and retrieval.

## 🗂️ Project Structure

project-folder/
│
├── index.php # Main file: form + table + logic
├── toggle.php # Handles AJAX request to toggle status
├── db.php # Database connection file
└── style.css # Optional CSS styling file


## 🧰 Setup Instructions

1. Install [XAMPP](https://www.apachefriends.org/) or any local server that supports PHP and MySQL.
2. Move the project folder to:
C:\xampp\htdocs\

pgsql
# Create the table:
USE form_demo;

CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100) NOT NULL,
  age INT NOT NULL,
  status TINYINT(1) DEFAULT 0
);
# Update db.php if your MySQL username or password is different.


# Access the app via browser
http://localhost/database/index.php
📸 Example
![صورة الداتابيس](https://github.com/user-attachments/assets/ccd13420-8a2c-417e-949f-efaac56e38db)


