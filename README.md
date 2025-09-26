# Ecommerce-MERN

Welcome to the **ecommerce-mern** project.  
This documentation serves as a technical guide for engineers, providing an in-depth understanding of the codebase, architecture, and integration points.  


This project leverages the **MERN stack**:  
- **MongoDB** for the database  
- **Express.js** for the backend framework  
- **React** for the frontend  
- **Node.js** as the runtime environment  



## 📂 Project Structure

```bash
ecommerce-mern/
│── client/   # React frontend (UI, routing, pages, components)
│── server/   # Node.js backend (API, models, controllers, middleware)
│── .env      # Environment variables
│── package.json
```

---

## ✨ Features

### 🔑 Authentication & Authorization

* User registration & login with hashed passwords
* JWT-based authentication
* Role-based access (User & Admin)

### 👨‍💼 Admin Features

* Category CRUD (Create, Read, Update, Delete)
* Product CRUD with image upload
* Manage orders & update order status

### 👤 User Features

* Browse products by category & price filters
* Search & pagination
* View product details & similar products
* Add to cart & checkout
* Manage profile & orders

### 🔒 Security

* Encrypted passwords with **bcrypt**
* JWT-protected routes
* Admin-only access controls

### 💳 Payment Integration

* Online payment gateway support


---

## 🏗️ Project Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/ecommerce-mern.git
cd ecommerce-mern
```

### 2️⃣ Setup Backend (server/)

```bash
cd server
npm install
```

* Create a `.env` file in `server/`:

```env
PORT=8080
MONGO_URL=your_mongo_connection_url
JWT_SECRET=your_jwt_secret
```

* Start the backend server:

```bash
npm start
```

### 3️⃣ Setup Frontend (client/)

```bash
cd client
npm install
npm start
```

* Frontend will run on → `http://localhost:3000`
* Backend will run on → `http://localhost:8080`

---

## 🔑 Authentication Flow

1. **Register** → User submits details → Password hashed → Saved in MongoDB
2. **Login** → JWT generated & returned → Stored in local storage
3. **Protected Routes** → Token verified by middleware (`requireSignIn`, `isAdmin`)

---
Architecture: 
<img width="562" height="747" alt="Screenshot 2025-09-22 165206" src="https://github.com/user-attachments/assets/d5ead771-6bd0-4473-bf25-0e542577198c" />


## 📸 Screenshots (Optional)

<img width="1213" height="404" alt="Screenshot 2025-09-16 144020" src="https://github.com/user-attachments/assets/e1749c53-6be8-4eb6-8db2-1a275f9e3ca1" />
<img width="1207" height="465" alt="Screenshot 2025-09-16 142615" src="https://github.com/user-attachments/assets/076109b2-e142-4e41-add8-25e882c6a0d8" />
<img width="1890" height="810" alt="Screenshot 2025-09-26 130452" src="https://github.com/user-attachments/assets/27aca720-48f5-43b7-b310-4d8f0eef8695" />
<img width="1144" height="805" alt="Screenshot 2025-09-26 125914" src="https://github.com/user-attachments/assets/0411400e-97f5-4a86-be46-bce1b3d708bf" />
<img width="534" height="752" alt="Screenshot 2025-09-26 125944" src="https://github.com/user-attachments/assets/9bf60c50-ec2c-4392-b142-427f4e80effe" />
<img width="1429" height="749" alt="Screenshot 2025-09-26 124058" src="https://github.com/user-attachments/assets/feb55300-73d5-4381-9ed4-3593e08d4506" />










