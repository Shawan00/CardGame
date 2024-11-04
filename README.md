Tại prj ĐoanSoClient thêm mysql-connector.jar và flatlaf.jar, download tại [đây](https://drive.google.com/drive/folders/1-Gx8yP4upc3OsxGSBXBjUopoZxn-hMq8?usp=drive_link)

Chạy lệnh trong mysql
```sql
CREATE DATABASE btlltm DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci;
USE btlltm;

CREATE TABLE users (
    userId INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(45) NOT NULL,
    password VARCHAR(45) NOT NULL,
    score FLOAT NOT NULL,
    win INT NOT NULL,
    draw INT NOT NULL,
    lose INT NOT NULL
);

CREATE TABLE history (
    id INT AUTO_INCREMENT PRIMARY KEY,
    userName1 VARCHAR(50),
    userName2 VARCHAR(50),
    resultMatch VARCHAR(200)
);
