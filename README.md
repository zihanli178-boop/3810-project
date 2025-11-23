#  Express Notes App with Facebook Authentication

This project is a Node.js web application built with **Express**, **Passport.js (Facebook OAuth)**, **MongoDB (Mongoose)**, and **Multer**.  
It allows users to log in via Facebook, manage notes (upload, search, update, delete, download), and view personalized content.

---

##  Features
-  **Facebook Login** using Passport.js
-  **Notes Management**:
  - Create notes with file uploads
  - Search notes by subject code
  - Update existing notes
  - Delete notes
  - Download uploaded files
-  **Session Management** with `express-session`
-  **File Uploads** handled by `multer`
-  **MongoDB Integration** using Mongoose
-  Views rendered with **EJS templates**

---

##  Tech Stack
- **Backend**: Node.js, Express
- **Authentication**: Passport.js (Facebook Strategy)
- **Database**: MongoDB Atlas (Mongoose ODM)
- **File Uploads**: Multer
- **Templating Engine**: EJS
- **Session Management**: express-session

## Installation
1. **clone the repository**
2. **install dependencies**
   **npm install**
3. **Configure environment variables**
4. **Run the application**
   **npm start**

## Project Structure
 .
├── models/
│   └── Note.js          # Mongoose schema for notes
├── public/              # Static assets (CSS, JS, images)
├── views/               # EJS templates (login, frontpage, search, list)
├── uploads/             # Uploaded files storage
├── app.js               # Main application file
└── README.md
 
## Authentication Flow
1. **User clicks Login with Facebook**
2. **Redirects to Facebook OAuth**
3. **On success → user session created → redirected to /content**
4. **On failure → redirected to /**

## Notes Management
1. **Create: Upload a file with subject code → stored in MongoDB**
2. **Search: Query notes by subject code**
3. **Update: Replace file for an existing note**
4. **Delete: Remove note from database**
5. **Download: Retrieve uploaded file**

## Acknowledgements
- **Express**
- **Passport.js**
- **Mongoose**
- **Multer**
- **EJS**

