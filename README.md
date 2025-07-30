# 📂 File Uploading System - Spring Boot Application

A Spring Boot-based REST API for uploading, downloading, and managing files. This project supports file validation, custom file naming, local storage and serves files securely with proper content types.

![Java](https://img.shields.io/badge/Java-17-blue.svg)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen.svg)
![Maven](https://img.shields.io/badge/Maven-Project-informational)
![Status](https://img.shields.io/badge/status-active-success)
![License](https://img.shields.io/github/license/your-username/file-upload-springboot)

---

## 🚀 Features

- Upload any file via REST API
- Parse file name, type and convert them into Java objects
- Save parsed data into the database
- Store the uploaded file in the file system
- Provide file download API

---

## 📦 Tech Stack

- Java 17+
- Spring Boot 3.x
- Spring Web
- Spring Data JPA
- H2 / PostgreSQL (any database of your choice)
- Lombok
- Maven
- Swagger

---

## 📂 Project Structure

```
src/
├── controller/
│   └── FileController.java
├── service/
│   └── FileService.java
├── helper/
│   └── FileHelper.java
├── model/
│   └── Files.java
├── repository/
│   └── FileRepository.java
└── ...
```

---

## 📤 How to Upload File

**Endpoint:**

```
POST /api/file/upload
```

**Form-File Body:**

- `file`: (type = `file`) Upload your file here.

---

## 📥 How to Download Uploaded File

**Endpoint:**

```
GET /api/file/download/{filename}
```

## 🛠️ How to Run Locally

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-repo/springboot-file-upload.git
   cd springboot-file-upload
   ```

2. **Configure DB (optional)**

   - For H2 (default): No setup needed
   - For PostgreSQL: Edit `application.properties`

3. **Run the application:**

   ```bash
   mvn spring-boot:run
   ```

4. **Access API Docs:**

   ```
   http://localhost:8080/swagger-ui/index.html
   ```

---

## 📎 Sample cURL Commands

### Upload File

```bash
curl -X POST http://localhost:8080/api/file/upload \
  -H "Content-Type: multipart/form-data" \
  -F "file=@/path/to/image.jpeg"
```

### Download Uploaded File

```bash
curl -O http://localhost:8080/api/file/download/image.jpeg
```

## 📬 Contact

For improvements or bug reports, please feel free to suggest any new term to make this application more robust.


