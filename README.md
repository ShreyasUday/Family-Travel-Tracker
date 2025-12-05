# 🧳 Family Travel Tracker — Backend Application (Node.js + Express + PostgreSQL)

The **Family Travel Tracker** is a backend-focused project designed to store and view family travel records using a PostgreSQL relational database. This application demonstrates the foundational backend concepts of **database connectivity, query execution, server-side rendering, and form handling** using Express and EJS.

---

## 🎯 Project Purpose

The goal of this project was to gain hands-on experience in:

- Understanding PostgreSQL relational database structures  
- Connecting Node.js applications securely to a database  
- Executing SQL queries from backend logic  
- Rendering dynamic UI based on database results  
- Handling form submissions to insert user-generated data  

This project served as an essential step before building full CRUD and API-based backend systems.

---

## 🚀 Core Features

- Add a new travel record through a form  
- View all travel entries stored in the database  
- Render dynamic data using EJS templates  
- Organized structure for scaling into full CRUD system  

---

## 🧰 Tech Stack

| Category | Tools |
|----------|------|
| Backend Runtime | Node.js |
| Web Framework | Express.js |
| Template Engine | EJS |
| Database | PostgreSQL |
| SQL Script | queries.sql |
| Version Control | Git & GitHub |

---

## 🗄 Database Schema & SQL Setup

The schema and SQL setup are included in the file:

📄 `queries.sql`

Example schema inside the project:

```sql
CREATE TABLE family_travel (
  id SERIAL PRIMARY KEY,
  name TEXT NOT NULL,
  country TEXT NOT NULL
);

psql -d your_database_name -f queries.sql
```

📁 Folder Structure
Family-Travel-Tracker/  
│── public/               # Static assets (CSS, images, client scripts)  
│── views/                # EJS templates  
│   ├── index.ejs         # List travel entries  
│   └── addTravel.ejs     # Form to add entry  
│── queries.sql           # Database creation & sample data  
│── index.js              # Express backend server  
│── package.json  
└── README.md

🔧 How to Run Locally

# Clone repository
git clone https://github.com/<your-username>/Family-Travel-Tracker.git

# Navigate into project
cd Family-Travel-Tracker

# Install dependencies
npm install

# Start the server
npm start

➡ Open in browser → http://localhost:3000

📌 What This Project Demonstrates (Backend Concepts)

✔ Database communication through Node.js  
✔ SQL query execution for SELECT & INSERT operations  
✔ Form handling and request processing  
✔ EJS-based server-side rendering  
✔ MVC-style separation of concerns (view + logic + DB)

🧭 Future Enhancements (Roadmap)

 Add UPDATE & DELETE features (Full CRUD)  
 Add login & role-based access for family members  
 Deploy project online (Render / Railway)  
 Replace EJS with React UI (optional)

🤝 Contributions

Contributions are welcome.
Improve the UI, extend CRUD, or introduce additional DB tables and submit a PR.
