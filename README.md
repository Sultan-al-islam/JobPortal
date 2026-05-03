# 💼 Job Portal - Full Stack Application

A modern, high-performance Job Portal built with the **MERN Stack** (MongoDB, Express, React, Node.js). This platform connects recruiters and job seekers, allowing users to post jobs, apply for positions, manage company profiles, and track application statuses in real-time.

---

## 🚀 Features

### For Job Seekers (Students)
- **User Authentication**: Secure signup and login with role-based access.
- **Profile Management**: Update personal details, skills, and upload resumes (via Cloudinary).
- **Job Search**: Browse and search for jobs with advanced filters (Location, Industry, Salary).
- **Applications**: Apply for jobs with a single click and monitor application status (Pending, Accepted, Rejected).

### For Recruiters
- **Company Registration**: Register and manage company profiles with logos.
- **Job Posting**: Create, edit, and manage job listings.
- **Applicant Tracking**: View all applicants for a specific job and update their status.
- **Dashboard**: Overview of posted jobs and company details.

---

## 🛠️ Tech Stack

### Frontend
- **Framework**: React.js with Vite
- **State Management**: Redux Toolkit & Redux Persist
- **Styling**: Tailwind CSS & Shadcn UI
- **Animations**: Framer Motion
- **Navigation**: React Router DOM
- **Icons**: Lucide React
- **Toast Notifications**: Sonner

### Backend
- **Runtime**: Node.js
- **Framework**: Express.js
- **Database**: MongoDB (Mongoose ODM)
- **Authentication**: JSON Web Token (JWT) with Cookie-parser
- **File Uploads**: Multer & Cloudinary
- **Environment Management**: Dotenv

---

## 📂 Project Structure

```text
jobportal/
├── backend/            # Express server, routes, controllers, and models
│   ├── controllers/    # Business logic for each route
│   ├── models/         # Mongoose schemas
│   ├── routes/         # API endpoints
│   ├── middlewares/    # Authentication and error handling
│   └── index.js        # Entry point
├── frontend/           # Vite + React application
│   ├── src/
│   │   ├── components/ # Reusable UI components (Shadcn)
│   │   ├── redux/      # Redux slices and store
│   │   ├── hooks/      # Custom React hooks
│   │   └── pages/      # Main page components
└── package.json        # Project scripts and dependencies
```

---

## ⚙️ Installation & Setup

### Prerequisites
- Node.js (v18 or higher)
- MongoDB Atlas account or local MongoDB
- Cloudinary account (for file uploads)

### 1. Clone the Repository
```bash
git clone https://github.com/Sultan-al-islam/JobPortal.git
cd jobportal
```

### 2. Backend Setup
Create a `.env` file in the root directory and add the following:
```env
MONGO_URI=your_mongodb_connection_string
PORT=8000
SECRET_KEY=your_jwt_secret
CLOUD_NAME=your_cloudinary_name
API_KEY=your_cloudinary_api_key
API_SECRET=your_cloudinary_api_secret
```

Install dependencies and start the server:
```bash
npm install
npm run dev
```

### 3. Frontend Setup
Navigate to the frontend directory:
```bash
cd frontend
npm install
npm run dev
```

The application will be running at `http://localhost:5173`.

---

## 🔒 Security
- Password hashing using **bcryptjs**.
- Protected routes using **JWT** stored in HTTP-only cookies.
- Middleware for role-based authorization.

---

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License
This project is licensed under the ISC License.

---
Developed with ❤️ by [Sultan-al-islam](https://github.com/Sultan-al-islam)
