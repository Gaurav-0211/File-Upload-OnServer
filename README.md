# 📂 File Uploading System - Spring Boot Application

A Spring Boot-based REST API for uploading, downloading, and managing files. This project supports file validation, custom file naming, local storage and serves files securely with proper content types.

![Java](https://img.shields.io/badge/Java-17-blue.svg)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen.svg)
![Maven](https://img.shields.io/badge/Maven-Project-informational)
![Status](https://img.shields.io/badge/status-active-success)
![License](https://img.shields.io/github/license/your-username/file-upload-springboot)

---

## 🚀 Tech Stack

- **Java 17**
- **Spring Boot 3.x**
- **Spring Web**
- **Lombok**
- **Apache Commons IO** (optional, for file type detection)
- **Swagger UI** for API documentation

---

## ✨ Features

- ✅ Upload single or multiple files via REST API
- ✅ Download files with correct MIME types
- ✅ Store files on local server disk (or modify for AWS S3, etc.)
- ✅ Auto-generate unique file names to prevent conflicts
- ✅ File size and type validation
- ✅ API documentation with Swagger UI

---

## 📁 Project Structure
### src/
### │
### ├── main/
### │ ├── java/com/fileupload/
### │ │ ├── controller/
### │ │ ├── service/
### │ │ ├── dto/
### | | |-- Entity/
### │ │ ├── config/
### │ │ └── FileUploadApplication.java
### │ └── resources/
### │ ├── application.properties
### │ └── static/



