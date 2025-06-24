# 📁 File Drive Clone

A minimal Google Drive–like file sharing app built with **Node.js**, **MongoDB**, and a simple frontend.

---

## 🚀 Version: 1.0.0

This is the **first stable release** of the File Drive Clone project. It includes core backend features with secure file handling, JWT authentication, MongoDB integration, and GitHub CodeQL alert automation.

---

## ✨ Features

- 🔐 User authentication (Register/Login using JWT)
- 📤 File upload support via `multer`
- 📁 Each user sees only their uploaded files
- 🔒 Secure download links with proper access control
- 🛡️ GitHub Webhook integration to auto-fix and dismiss CodeQL alerts
- 🧠 CodeQL and express-rate-limit security enhancements
- ☁️ MongoDB Atlas integration
- 📦 Deploy-ready (Tested on Render and Fly.io)
- 💡 Clean architecture and `.env.example` included

---

## 📂 Folder Structure
fileshare/ ├── backend/ │ ├── bot/ # GitHub automation bot (fix + dismiss CodeQL) │ ├── middleware/ # Rate limiter │ ├── models/ # Mongoose schemas (User, File) │ ├── routes/ # Auth and file routes │ ├── uploads/ # Uploaded file storage │ ├── server.js # Entry point │ └── package.json # Backend dependencies ├── frontend/ │ ├── css/ # Basic styles │ ├── js/ # Client-side JS (upload, auth) │ ├── index.html # Homepage / file listing │ ├── login.html # Login page │ └── register.html # Register page ├── .gitignore ├── .env.example # Environment variable template ├── README.md └── CHANGELOG.md
---

## 🧪 Technologies Used

- **Node.js**
- **Express**
- **MongoDB Atlas**
- **Mongoose**
- **JWT (jsonwebtoken)**
- **Multer**
- **GitHub Webhooks**
- **Octokit (GitHub Bot API)**

---

## 🛠️ Getting Started

### 1. Clone the Repo
```bash
git clone https://github.com/your-username/fileshare_backend.git
cd fileshare
```
2. Install Backend Dependencies
```bash
cd backend
npm install
```
###3. Configure Environment Variables

Create a .env file in the root of the backend/ directory and copy from .env.example.

3. Run the Backend Server
```bash
npm start
```
4. Open the Frontend
Open frontend/index.html in your browser.

📌 Notes
Ensure MongoDB Atlas URI is set correctly in .env

JWT secret and GitHub Webhook secret must be securely stored

Designed to work out of the box on Render and Fl
