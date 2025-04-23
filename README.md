# 🧪 Chemical Inventory Management System

A MERN stack-based application built for managing chemical inventory at S.S. Enterprises Pvt. Ltd. The system provides full CRUD capabilities for chemicals, purchases, sales, and safety information, with user roles (admin and staff), reporting features, and secure authentication.

---

## 🔧 Tech Stack

- **Frontend**: React + Vite, React Router, Axios, Bootstrap/React-Bootstrap  
- **Backend**: Node.js, Express.js, MongoDB, Mongoose  
- **Authentication**: JWT, bcrypt  
- **Deployment**:  
  - **Frontend**: AWS S3  
  - **Backend**: AWS EC2  
  - **Database**: MongoDB Atlas or AWS RDS  
  - **CI/CD**: GitHub + AWS CodeBuild (Optional)

---

## 📁 Project Structure

Chemical_inventory/ ├── backend/ # Express.js server, routes, models, controllers ├── frontend/ # React frontend built with Vite ├── .env # Environment variables └── README.md # Project documentation

yaml
Copy
Edit

---

## 🚀 Features

### 👨‍💼 Authentication & Roles
- Role-based access (Admin, Warehouse Staff)
- Secure JWT-based login and registration
- Automatic role assignment (First user becomes Admin)

### 📦 Inventory Management
- CRUD operations for Chemicals, Purchases, Sales, Safety data
- React forms with validations
- User-friendly dashboards with summary stats

### 📊 Reporting
- Detailed reports combining chemical, purchase, and sales data
- Export reports in CSV format

---

## 🛠️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/chemical-inventory.git
cd chemical-inventory
2. Backend Setup
bash
Copy
Edit
cd backend
npm install
cp .env.example .env
# Update .env with your MongoDB URI, JWT_SECRET, etc.
npm run dev
3. Frontend Setup
bash
Copy
Edit
cd ../frontend
npm install
npm run dev
🌐 Deployment (AWS)
Frontend (S3 + CI/CD)
Upload Vite build output to AWS S3

Use AWS CodeBuild + GitHub for automatic deployment

Ensure API base URL points to EC2 backend

Backend (EC2)
SSH into an EC2 instance

Install Node.js, MongoDB client, and PM2

Deploy backend/ and run the server on port 5000 using PM2

🔐 Environment Variables
.env (Backend)
ini
Copy
Edit
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
📸 Screenshots
Add UI screenshots here once ready.

📄 License
This project is licensed under the MIT License.

