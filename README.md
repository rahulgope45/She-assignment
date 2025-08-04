She-Can (Local Development Setup)
Overview
This project is a full-stack web application built with:

Frontend: React + Vite (Port 5173)

Backend: Node.js + Express (Port 8080)

Database: MongoDB Atlas (Cloud)

This README provides steps to set up locally for development and testing.

Features
User authentication (signup/login/logout) with sessions

Donation management (add/view donations)

Responsive design with TailwindCSS

MongoDB Atlas cloud database

Tech Stack

Frontend --->
React
React Router DOM
Axios
Tailwind CSS

Backend --->
Express
MongoDB (Mongoose)
express-session
bcrypt (password hashing)
connect-mongo (session storage)

Backend (server/)
npm install express mongoose cors bcrypt dotenv express-session connect-mongo nodemon axios

Frontend (client/)
npm install react react-dom react-router-dom axios
npm install -D tailwindcss postcss autoprefixer vite


Environment Variables
Create .env in server/:
PORT=8080
MONGO_URI="mongodb+srv://<username>:<password>@<cluster>.mongodb.net/userCredentials"
FRONTEND_URL=http://localhost:5173
SESSION_SECRET=123rahul
NODE_ENV=development

API Endpoints
Auth
POST /signup → Create new user
POST /login → Login user
GET /user → Get logged-in user

POST /logout → Logout user
Donations
GET /donations
POST /donations

Screenshots / Proof
<img width="1919" height="861" alt="Screenshot 2025-08-04 185910" src="https://github.com/user-attachments/assets/c7e51e0b-fdfb-4677-ac0b-0cfb0660f41f" />
<img width="1919" height="869" alt="Screenshot 2025-08-04 221630" src="https://github.com/user-attachments/assets/6d70b194-6017-44e7-a0ac-9508f5cceb2c" />
