# 🎙️ Voice Assistant Bot

## 📌 Project Overview

This project is a web-based Voice Assistant Bot developed using HTML, CSS, JavaScript, and PHP. The application allows users to communicate with an AI assistant through a simple and interactive interface. The frontend collects the user's input, while the PHP backend processes the request and sends it to the AI API before returning the generated response.

---

# 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript
- PHP
- XAMPP
- Groq API
- Git
- GitHub

---

# 🚀 Part 1 – Uploading the Project to the Server

The project was deployed on a local server using XAMPP.

### Steps Performed

1. Installed and configured XAMPP.
2. Started the Apache service.
3. Created a project folder named **BOT** inside the **htdocs** directory.
4. Copied all frontend and backend files into the project folder.
5. Verified that all file paths were correct.
6. Opened the application using:

```
http://localhost/BOT/
```

7. Confirmed that the interface loaded successfully before testing the chatbot functionality.

---

# 🔧 Part 2 – Fixing the PHP File

## Problem Description

Initially, whenever the user attempted to send a message, the application displayed:

```
حدث خطأ أثناء الاتصال بالخادم، حاول مجدداً
```

This indicated that the frontend was unable to receive a valid response from the backend.

---

## 🔍 Troubleshooting Process

To identify the cause of the issue, several debugging steps were performed:

- Verified that Apache was running correctly.
- Checked the project folder location inside the XAMPP server.
- Confirmed that all project files were uploaded correctly.
- Tested the PHP endpoint separately in the browser.
- Verified that POST requests were reaching the PHP file.
- Inspected the browser Developer Tools (Network & Console).
- Confirmed that JavaScript was sending requests to the correct API endpoint.
- Checked the HTTP response codes returned by the server.
- Tested JSON request and response formatting.
- Verified the API key configuration.
- Tested communication with the external AI service.
- Reviewed PHP error handling and response formatting.
- Checked cURL requests and API authentication.
- Verified file paths and configuration files.
- Replaced incorrect API configuration with the correct one.
- Migrated the project from Gemini API to Groq API after API quota limitations prevented successful requests.

---

## ✅ Solution

Several modifications were made to the PHP backend:

- Configured the endpoint to accept only POST requests.
- Added input validation before processing requests.
- Improved JSON request parsing.
- Added proper HTTP status codes.
- Implemented better error handling for API requests.
- Configured secure communication with the Groq API.
- Returned structured JSON responses to the frontend.
- Verified successful communication between JavaScript and PHP.

After applying these changes, the chatbot was able to communicate successfully with the AI service.

---

# 🔑 API Configuration

The API key is stored inside:

```
config.php
```

For security reasons, the actual API key has been removed from this repository.

Example:

```php
define('GROQ_API_KEY', 'YOUR_API_KEY');
```

---

# 📂 Part 3 – GitHub Documentation

After completing the implementation and debugging process, the project was uploaded to GitHub.

The repository includes:

- HTML files
- CSS files
- JavaScript files
- PHP backend
- Configuration file
- README documentation
- Demo video

---

# ✨ Features

- Voice assistant interface
- Responsive web design
- AI-powered chatbot
- PHP backend integration
- Secure API communication
- JSON request handling
- Error handling
- Local server deployment

---

# ⚠️ Challenges Faced

Throughout the project, several technical issues were encountered:

- Incorrect API endpoint configuration.
- Backend connection failures.
- Invalid POST request handling.
- JSON parsing errors.
- API authentication problems.
- Gemini API quota limitations.
- HTTP 405 and 502 server errors.
- cURL communication issues.
- Incorrect file paths.
- PHP configuration errors.
- JavaScript request validation.
- Local server configuration issues.
- Debugging frontend-backend communication.
- Verifying API responses and status codes.

Each issue was analyzed using browser Developer Tools, PHP debugging techniques, and server-side testing until the application functioned correctly.

---

# ✅ Final Result

The project was successfully deployed on a local server, the PHP communication issue was resolved, the chatbot was integrated with the Groq API, and the final project was uploaded to GitHub with complete documentation and demonstration files.

---

# 👩‍💻 Author

**Ebtihal Al-Amri**

Computer and Network Engineering Student

University of Jeddah
