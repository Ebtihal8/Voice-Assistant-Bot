# Voice-Assistant-Bot

## Project Overview

This project is a web-based Voice Assistant Bot that allows users to interact with an AI assistant through a simple web interface. The project consists of HTML, CSS, JavaScript, and PHP files. The PHP backend receives requests from the frontend and communicates with the AI API to generate responses.

---

# Project Structure

```
BOT/
│
├── api/
│   └── chat.php
│
├── index.html
├── app.js
├── style.css
├── config.php
├── .htaccess
└── README.md
```

---

# Technologies Used

- HTML5
- CSS3
- JavaScript
- PHP
- XAMPP (Local Server)
- Groq API
- Git & GitHub

---

# Part 1 – Uploading Project Files

The project was uploaded to a local server using **XAMPP**.

### Steps

1. Installed and started Apache using XAMPP.
2. Created a project folder named **BOT** inside:

```
C:\xampp\htdocs\
```

3. Copied all project files into the folder.

4. Opened the project in the browser using:

```
http://localhost/BOT/
```

The website loaded successfully.

---

# Part 2 – Fixing the PHP File

## Problem

When sending a message from the chatbot, the following error appeared:

```
حدث خطأ أثناء الاتصال بالخادم، حاول مجدداً
```

This happened because the PHP file responsible for handling requests and communicating with the AI API was not working correctly.

---

## Investigation

The following checks were performed:

- Verified the project structure.
- Verified the API request path.
- Checked the POST request.
- Tested the PHP endpoint.
- Inspected browser Developer Tools.
- Checked Network requests.
- Tested API responses.

---

## Solution

The PHP file (**chat.php**) was modified to:

- Accept only POST requests.
- Read JSON data correctly.
- Validate the input prompt.
- Connect to the AI API securely.
- Return JSON responses.
- Handle HTTP and cURL errors properly.

The project was also migrated from **Gemini API** to **Groq API** after encountering API quota limitations.

---

# API Configuration

The API key is stored inside:

```
config.php
```

Example:

```php
define('GROQ_API_KEY', 'YOUR_API_KEY');
```

The real API key is not included in this repository for security reasons.

---

# Part 3 – GitHub Repository

After completing the fixes:

- Created a GitHub repository.
- Uploaded all project files.
- Added this README file.
- Uploaded a demonstration video of the project.

Repository contents include:

- index.html
- style.css
- app.js
- chat.php
- config.php (without the real API key)
- .htaccess
- README.md
- Demo video

---

# Features

- Voice Assistant Interface
- Responsive Design
- JavaScript Frontend
- PHP Backend
- API Integration
- JSON Communication
- Error Handling

---

# Challenges

During development, several issues were encountered:

- Incorrect API endpoint.
- API quota exceeded while using Gemini.
- PHP request validation.
- Backend connection errors.
- API authentication issues.

These issues were diagnosed using browser Developer Tools and resolved successfully.

---

# Result

The chatbot project was successfully deployed on a local server, the PHP backend was fixed, the API integration was completed, and the final project was uploaded to GitHub with full documentation.

---

# Author

**Ebtihal Al-Amri**

Computer and Network Engineering Student

University of Jeddah
