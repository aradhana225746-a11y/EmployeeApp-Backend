# Employee App - Backend Integration

This project is a Full-Stack Employee Management Application with an Angular frontend (pre-compiled build inside `dist/Frontend`) integrated with a Node.js/Express and MongoDB Atlas backend.

---

## 🚀 Features & API Implementation

All backend logic is implemented in [app.js](file:///C:/Users/Rose/.gemini/antigravity/scratch/EmployeeApp/Casestudy2/app.js) while strictly preserving all predefined comments and starter code.

| HTTP Method | Endpoint | Description | Request Body Format |
|---|---|---|---|
| **GET** | `/api/employeelist` | Fetch all employees from MongoDB Atlas | None |
| **GET** | `/api/employeelist/:id` | Fetch single employee details by ID | None |
| **POST** | `/api/employeelist` | Add a new employee | `{ "name": "John Doe", "location": "New York", "position": "Developer", "salary": 60000 }` |
| **PUT** | `/api/employeelist` | Update an existing employee | `{ "_id": "<id>", "name": "John Doe", "location": "California", "position": "Lead", "salary": 75000 }` |
| **DELETE** | `/api/employeelist/:id` | Delete an employee by ID | None |
| **GET** | `/*` | Serves the frontend Angular build (`dist/Frontend/index.html`) | None |

---

## 🛠️ Tech Stack & Dependencies

- **Node.js** (Runtime environment)
- **Express.js** (Backend web framework)
- **Mongoose** (MongoDB ODM)
- **Cors** (Cross-origin resource sharing middleware)
- **Dotenv** (Environment variable management)
- **Angular** (Pre-compiled SPA frontend in `dist/Frontend`)

---

## ⚙️ Installation & Setup Instructions

### 1. Prerequisites
- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- MongoDB Atlas account and cluster connection URI

### 2. Install Dependencies
Open a terminal in the project directory (`Casestudy2`) and run:
```bash
npm install
```

### 3. Configure MongoDB Atlas Connection
Create a `.env` file in the root directory (or update the provided one):
```env
MONGODB_URI=your_mongodb_atlas_connection_string
PORT=3000
```
> **Note:** Configure your Atlas connection string inside `.env`. The `.env` file is excluded from Git tracking via `.gitignore` for security.

### 4. Run the Application
Start the server:
```bash
npm start
```
Or directly with Node:
```bash
node app.js
```

### 5. Access the Application
Open your browser and navigate to:
```
http://localhost:3000
```

---

## 📁 Project Structure

```
Casestudy2/
├── app.js               # Express application with all CRUD APIs & DB connection
├── package.json         # Node.js dependencies and start script
├── .env.example         # Template for environment variables
├── .gitignore           # Ignores node_modules and .env
├── README.md            # Project documentation and guide
└── dist/
    └── Frontend/        # Compiled Angular application build
```

---

## 📤 Pushing to GitHub

To submit your GitHub repository link:
1. Initialize git in the project root:
   ```bash
   git init
   git add .
   git commit -m "Complete Employee App backend integration"
   ```
2. Create a new repository on [GitHub](https://github.com/new).
3. Link the remote and push:
   ```bash
   git remote add origin https://github.com/<your-username>/<your-repo-name>.git
   git branch -M main
   git push -u origin main
   ```
4. Copy the repository URL and submit it.
