# 🚗 Garasifyy - Car Modification Management System

Website dan API untuk mengelola data modifikasi mobil, customer, project, dan services.

**Author:** 23552011045_Luthfy Arief_TIF_RP_23_CNS_A  
**Version:** 1.0.0  
**Tech Stack:** HTML, CSS, JavaScript, Node.js, Express.js

---

## 🚀 Quick Start

### Frontend Website
```bash
# Buka file di browser
index.html         # Homepage
dashboard.html     # Admin Dashboard  
login.html        # Login Page
register.html     # Register Page
detail.html       # Car Detail Page
```

### Backend API
```bash
cd api
npm install
npm start

# Server berjalan di: http://localhost:3000
```

---

## 🌟 Features

### Frontend
- ✅ **Modern UI/UX** dengan tema modifikasi mobil
- ✅ **Responsive Design** untuk semua device
- ✅ **Interactive Dashboard** dengan statistik
- ✅ **Car Gallery** dan testimonials
- ✅ **Login/Register** system

### Backend API
- ✅ **RESTful API** dengan Express.js
- ✅ **Complete CRUD** untuk Cars, Customers, Projects, Services
- ✅ **Authentication** system
- ✅ **Pagination & Filtering**
- ✅ **Statistics & Analytics**

---

## 📡 API Endpoints

### Base
- `GET /` - API Information
- `GET /health` - Health Check

### Authentication
- `POST /api/auth/login` - Login
- `POST /api/auth/register` - Register

### Cars
- `GET /api/cars` - Get all cars
- `POST /api/cars` - Create new car
- `PUT /api/cars/:id` - Update car
- `DELETE /api/cars/:id` - Delete car
- `GET /api/cars/stats/summary` - Car statistics

### Customers
- `GET /api/customers` - Get all customers
- `POST /api/customers` - Create customer
- `GET /api/customers/loyalty/top` - Top customers

### Projects
- `GET /api/projects` - Get all projects
- `POST /api/projects` - Create project
- `GET /api/projects/stats/dashboard` - Project stats

### Services
- `GET /api/services` - Get all services
- `POST /api/services` - Create service
- `GET /api/services/popular/list` - Popular services

---

## 🧪 Testing

### Demo Credentials
```json
{
  "email": "user@utb.ac.id",
  "password": "utsweb1"
}
```

### Sample Requests

**Get All Cars:**
```bash
GET http://localhost:3000/api/cars
```

**Create Car:**
```bash
POST http://localhost:3000/api/cars
Content-Type: application/json

{
  "brand": "Toyota",
  "model": "Supra MK4",
  "year": 1998,
  "owner": "Test User",
  "color": "Deep Blue Metallic",
  "engine": "2JZ-GTE",
  "horsepower": 320,
  "modifications": ["Turbo Upgrade", "Exhaust System"],
  "estimatedValue": 850000000
}
```

**Login:**
```bash
POST http://localhost:3000/api/auth/login
Content-Type: application/json

{
  "email": "user@utb.ac.id",
  "password": "utsweb1"
}
```

---

## 📊 Data Models

**Car:**
```json
{
  "id": "uuid",
  "brand": "Toyota",
  "model": "Supra MK4", 
  "year": 1998,
  "owner": "Ahmad Rizki",
  "engine": "2JZ-GTE",
  "horsepower": 320,
  "modifications": ["Turbo Upgrade"],
  "status": "completed",
  "estimatedValue": 850000000
}
```

**Customer:**
```json
{
  "id": "uuid",
  "name": "Ahmad Rizki",
  "email": "ahmad@email.com",
  "phone": "+62812345678",
  "totalProjects": 3,
  "loyaltyPoints": 1250
}
```

---

## 📁 Project Structure

```
garasifyy/
├── index.html              # Homepage
├── dashboard.html          # Admin Dashboard
├── login.html             # Login Page
├── register.html          # Register Page
├── detail.html            # Car Detail Page
├── css/
│   └── style.css          # Styling
├── js/
│   └── script.js          # Frontend Logic
├── api/
│   ├── server.js          # Express Server
│   ├── package.json       # Dependencies
│   ├── routes/            # API Routes
│   │   ├── cars.js
│   │   ├── customers.js
│   │   ├── projects.js
│   │   ├── services.js
│   │   └── auth.js
│   └── data/
│       └── dummy-data.js  # Sample Data
├── screenshots/           # API Screenshots
├── Garasifyy_API_Collection.postman_collection.json
└── README.md
```

---

## 🎯 Usage

1. **Frontend Development:**
   - Open `index.html` in browser
   - Navigate through different pages
   - Test responsive design

2. **API Development:**
   - Start server: `cd api && npm start`
   - Test endpoints with Postman
   - Import collection for easy testing

3. **Full-Stack Testing:**
   - Run API server
   - Open frontend in browser
   - Test integration between frontend and API

---

## 👨‍💻 Developer

**23552011045_Luthfy Arief_TIF_RP_23_CNS_A**  
*Universitas Teknologi Batam*  
*Program Studi Teknik Informatika*

---

## 📞 Contact

- Email: luthfy.arief@student.utb.ac.id
- GitHub: [Repository Link](https://github.com/tech0608/Garasifyy_UTS_Web1)

---

*© 2025 Garasifyy. All rights reserved.*