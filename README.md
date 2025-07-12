
# 📄 Online Marriage Registration System

This project is an **Online Marriage Registration Portal** developed in **PHP**, **HTML**, **CSS**, **JavaScript**, and **MySQL**.

It allows:
- Users to register their marriage details online.
- Admin to review and approve registrations.
- Users to track the status of their application.

---

## 🚀 Features

✅ User Registration  
✅ Marriage Registration Form  
✅ Application Status Tracking  
✅ Admin Panel for Approval  
✅ Dashboard & Reports

---

## 🖥️ Requirements

- **XAMPP** (or any other local server stack with Apache, PHP & MySQL)  
- Web browser (Chrome, Firefox, Edge, etc.)

---

## ⚙️ How to Install & Run

Follow these steps to set up the project on your local machine:

### 1️⃣ Install XAMPP

- Download XAMPP from [Apache Friends](https://www.apachefriends.org/index.html).
- Install it and start **Apache** and **MySQL** from the **XAMPP Control Panel**.

---

### 2️⃣ Setup the Project Files

1. Extract the `MiniProject.zip` file.  
2. Copy the extracted project folder (e.g., `MiniProject`) to the `htdocs` directory of your XAMPP installation.  
   - Example path: `C:\xampp\htdocs\MiniProject`

---

### 3️⃣ Create the Database

1. Open your web browser and go to: [http://localhost/phpmyadmin](http://localhost/phpmyadmin)  
2. Click **Databases** tab.  
3. Create a new database. For example, name it: `marriage_db`.  
4. Import the project SQL file:
   - Click your newly created database name.
   - Click **Import** tab.
   - Click **Choose File** and select the `.sql` file included in your project (check inside your extracted folder).
   - Click **Go** to import the database tables.

---

### 4️⃣ Configure Database Connection

1. Open the project folder in a code editor (VS Code, Sublime, Notepad++).  
2. Find the file where the database configuration is written — usually named `config.php` or `db.php`.  
3. Make sure the database details are correct:

   ```php
   <?php
   $servername = "localhost";
   $username = "root";
   $password = "";
   $dbname = "marriage_db"; // Replace with your database name
   $conn = mysqli_connect($servername, $username, $password, $dbname);
   if (!$conn) {
       die("Connection failed: " . mysqli_connect_error());
   }
   ?>
   ```

   - By default, XAMPP uses username **root** with an empty password.

---

### 5️⃣ Access the Application

1. Open your browser and go to:  
   ```
   http://localhost/MiniProject/
   ```
   or if you renamed the folder:  
   ```
   http://localhost/your-folder-name/
   ```

2. Register as a user or log in as an admin (default credentials if provided).

---

## ✅ Done!

You now have your **Online Marriage Registration System** running locally!  
Feel free to customize it and add new features.

---

