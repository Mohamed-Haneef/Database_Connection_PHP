# INTRODUCTION
Database connection tool built using PHP and MySQL. Designed to simplify and optimize the process of establishing and managing database connections in web applications.
This project provides a robust and user-friendly solution, addressing the challenges developers often face when handling database connectivity.
# INSTALLATION

Clone the repository using the following command:

```bash
git clone https://github.com/Mohamed-Haneef/Database_Connection_PHP  
```
(Free source code!!)

# CONFIGURATION
### config.php
    $__site_config_path = $_SERVER['DOCUMENT_ROOT'] . '/../config.json';
It is preferred to keep the database credentials outside the `DOCUMENT_ROOT` of your server. (It is a good practice).
### config.json
    {
      "DB_SERVER": "Database_server_name",
      "DB_USER": "Database_username",
      "DB_PASSWORD": "Database_Password",
      "DB_NAME": "database_name"
    }
# USAGE
Whenever you want to use the database, all you have to do is to follow these simple steps.<br><br>

### Step 1:
    include '/path/database.class.php';
Including the 'database.class.php' file.

### Step 2:
    $conn = Database::getConnection();
Initiating the database connection by declaring a variable named 'conn' (it can also be an object class or instance).

### Step 3:
Write the MySQL Queries as per needed.

### Step 4:
    $conn = Database::closeConnection();
Close the database connection once the required values are modified.
> Warning: Not closing the database connection could lead to a serious vulnerability.

# License
Free source - No copyrights claimed.
