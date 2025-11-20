# 🔧 Garasify - Platform Modifikasi Mobil Premium

**UTS Web Programming 1**  
**TIF RP-23 CNS A**  
**Nama: [Nama Anda]**  
**NIM: [NIM Anda]**

## 📋 Deskripsi Project

Garasify adalah platform digital yang menyediakan layanan modifikasi mobil premium dengan teknologi terdepan. Website ini dibangun sebagai tugas UTS Web Programming 1 dengan fokus pada pengembangan frontend web application menggunakan HTML5, CSS3, Bootstrap, dan JavaScript dengan integrasi backend API menggunakan Node.js dan Express.

## ✨ Fitur Utama

### 🏠 Landing Page
• **Hero Section** - Tampilan utama dengan animasi partikel yang menarik
• **Service Gallery** - Galeri layanan utama (Engine Performance, Wide Body, Interior & Audio)
• **About Section** - Informasi tentang Garasify dan layanan premium
• **Contact Section** - Informasi kontak dan lokasi workshop

### 🔧 Service Pages
• **Engine Performance** - Layanan upgrade performa mesin dan turbocharger
• **Wide Body Modification** - Modifikasi body kit ekstrem dan custom paint
• **Interior & Audio** - Upgrade interior luxury dan sistem audio premium
• **Detail Information** - Informasi lengkap setiap layanan dengan galeri

### 👤 User System
• **User Registration** - Pendaftaran akun baru dengan validasi
• **User Login** - Sistem login dengan session management
• **User Dashboard** - Halaman dashboard personal untuk user yang login
• **Profile Management** - Manajemen profil dan informasi user

### 🔌 REST API Backend
API endpoints untuk operasi CRUD:
• `GET /api/services` - Mengambil data layanan
• `POST /api/auth/register` - Registrasi user baru
• `POST /api/auth/login` - Login user
• `GET /api/customers` - Data customer
• `GET /api/projects` - Data project modifikasi

## 🛠 Teknologi yang Digunakan

### Frontend
• **HTML5** - Struktur web modern dengan semantic elements
• **CSS3** - Advanced styling dengan custom properties, animations, dan gradients
• **Bootstrap 5.3.2** - Framework CSS untuk responsive design
• **JavaScript (Vanilla)** - Interactive elements, particle animations, dan form validation
• **Font Awesome 6.4.0** - Icon library untuk UI enhancement

### Backend
• **Node.js** - Runtime environment untuk server-side JavaScript
• **Express.js** - Web framework untuk API development
• **JSON** - Data storage untuk development phase

### Development Tools
• **Laragon** - Local development environment
• **Git & GitHub** - Version control system
• **VS Code** - Code editor dengan extensions

## 📁 Struktur Project

```
utsweb1/
├── api/                        # Backend API
│   ├── package.json           # Dependencies configuration
│   ├── server.js              # Express server setup
│   ├── data/
│   │   └── dummy-data.js      # Sample data untuk development
│   └── routes/
│       ├── auth.js            # Authentication routes
│       ├── cars.js            # Car data routes  
│       ├── customers.js       # Customer routes
│       ├── projects.js        # Project routes
│       └── services.js        # Service routes
├── css/                       # Stylesheets
│   ├── style.css              # Main stylesheet dengan advanced CSS
│   └── form-fixes.css         # Form styling fixes
├── js/                        # JavaScript files
│   └── script.js              # Main script dengan particle animations
├── index.html                 # Homepage utama
├── login.html                 # Login page
├── register.html              # Registration page  
├── dashboard.html             # User dashboard
├── detail.html                # Service detail page
└── README.md                  # Project documentation
```

## 🗄 Database Schema

### Sample Data Structure

#### Services Data
```json
{
  "id": "engine-performance",
  "title": "Engine Performance",
  "description": "Upgrade performa mesin dengan teknologi terdepan",
  "price": "Mulai dari Rp 15.000.000",
  "image": "engine-photo.jpg",
  "features": ["Turbo Installation", "ECU Remapping", "Exhaust System"]
}
```

#### Customer Data
```json
{
  "id": "customer-001",
  "name": "Ahmad Rizki",
  "email": "ahmad@email.com",
  "phone": "+62812345678",
  "registeredAt": "2024-01-15"
}
```

#### Project Data
```json
{
  "id": "project-001", 
  "customerName": "Ahmad Rizki",
  "carModel": "Toyota Supra",
  "serviceType": "Engine Performance",
  "status": "In Progress",
  "totalCost": 25000000
}
```

## 🚀 Instalasi dan Setup

### 1. Prerequisites
• Node.js 18.x atau lebih tinggi
• npm atau yarn package manager
• Web browser modern (Chrome, Firefox, Safari, Edge)
• Text editor (VS Code recommended)

### 2. Clone Repository
```bash
git clone https://github.com/tech0608/Garasifyy_UTS_Web1.git
cd utsweb1
```

### 3. Backend Setup
```bash
cd api
npm install
npm start
```

### 4. Configuration
Update pengaturan server di `api/server.js`:
```javascript
const PORT = process.env.PORT || 3000;
const HOST = 'localhost';
```

### 5. Run Application
• **Frontend**: Buka `index.html` di browser atau gunakan live server
• **Backend**: Akses via `http://localhost:3000`

## 📱 Responsive Design

Website ini dioptimalkan untuk berbagai ukuran layar:
• **Desktop (1200px+)** - Full layout dengan advanced animations
• **Tablet (768px - 1199px)** - Adapted layout dengan optimized spacing
• **Mobile (< 768px)** - Mobile-first design dengan touch-optimized interface

## 🔒 Security Features

• **Client-side Validation** - Form validation dengan JavaScript
• **Input Sanitization** - Clean user input untuk security
• **Session Management** - Proper session handling untuk authentication
• **Responsive Security** - Mobile-friendly security implementation
• **Modern Standards** - Implementation mengikuti web security best practices

## 🎨 Design System

### Color Palette
• **Primary**: `#ff0040` (Vibrant Red) - Brand color untuk CTA dan highlights
• **Secondary**: `#000000` (Pure Black) - Text dan navigation
• **Accent**: `#ffffff` (White) - Background dan contrast
• **Gradient**: `linear-gradient(135deg, #ff0040 0%, #ff4081 100%)` - Modern gradient effects

### Typography
• **Primary Font**: Inter (Google Fonts) - Modern sans-serif untuk body text
• **Heading Font**: Poppins (Google Fonts) - Bold headings dengan excellent readability
• **Icon Font**: Font Awesome 6 - Comprehensive icon library

### Visual Effects
• **Particle Animation** - Interactive background particles untuk engagement
• **Smooth Transitions** - CSS transitions untuk better UX
• **Responsive Cards** - Modern card design dengan hover effects
• **Glass Morphism** - Modern UI dengan backdrop-blur effects

## 📊 API Documentation

### Authentication Endpoints

#### POST /api/auth/register
Registrasi user baru.

**Body:**
```json
{
  "name": "John Doe",
  "email": "john@example.com", 
  "password": "securePassword123",
  "phone": "081234567890"
}
```

#### POST /api/auth/login
Login user existing.

**Body:**
```json
{
  "email": "john@example.com",
  "password": "securePassword123"
}
```

### Service Endpoints

#### GET /api/services
Mengambil data semua layanan.

**Response:**
```json
{
  "services": [
    {
      "id": "engine-performance",
      "title": "Engine Performance",
      "description": "Upgrade performa mesin dengan teknologi terdepan",
      "price": "Mulai dari Rp 15.000.000"
    }
  ]
}
```

#### GET /api/customers
Mengambil data customer.

#### GET /api/projects  
Mengambil data project modifikasi.

#### GET /api/cars
Mengambil data mobil yang dimodifikasi.

**Response:**
```json
{
  "cars": [
    {
      "id": "car-001",
      "brand": "Toyota",
      "model": "Supra MK4",
      "year": 1998,
      "modifications": ["Turbo Upgrade", "Body Kit"],
      "status": "completed"
    }
  ]
}
```

## 🎯 Fitur Unggulan

### Interactive Elements
• **Particle Background** - Animated particles untuk visual appeal
• **Smooth Scrolling** - Enhanced user experience dengan smooth navigation
• **Dynamic Content** - JavaScript-powered content loading
• **Responsive Gallery** - Touch-friendly image gallery

### Modern UI/UX
• **Card-based Design** - Clean dan modern card layout
• **Micro-animations** - Subtle animations untuk better engagement  
• **Loading States** - User feedback untuk better experience
• **Error Handling** - Graceful error handling dengan user-friendly messages

## 🏆 Best Practices Implementation

• **Semantic HTML** - Proper HTML5 semantic elements
• **Accessible Design** - WCAG compliance untuk accessibility
• **SEO Optimization** - Meta tags dan structured data
• **Performance** - Optimized images dan efficient code
• **Mobile-First** - Mobile-first responsive design approach

## 🧪 Testing

### Demo Credentials
```json
{
  "email": "user@garasify.com",
  "password": "garasify123"
}
```

### Sample API Requests

**Create New Service:**
```bash
POST http://localhost:3000/api/services
Content-Type: application/json

{
  "title": "Suspension Upgrade",
  "description": "Premium coilover dan stabilizer upgrade",
  "price": "Rp 12.000.000",
  "category": "performance"
}
```

**Get Customer Data:**
```bash
GET http://localhost:3000/api/customers
Authorization: Bearer <token>
```

## 👨‍💼 Team

**Developer & Designer:** [Nama Anda]
- Frontend Development
- UI/UX Design  
- Backend API Development
- Project Management

## 📞 Kontak

• **Email:** info@garasify.com
• **Website:** [Garasify Local](http://localhost/utsweb1)
• **GitHub:** [tech0608](https://github.com/tech0608)
• **Workshop:** Jl. Modifikasi Premium No. 123, Jakarta

## 📝 License

This project is created for educational purposes as part of UTS Web Programming 1 assignment.

**Developed with ❤️ by [Nama Anda]**  
**Universitas Teknologi Bandung (UTB)**

---

© 2024 Garasify - Premium Car Modification Platform. All rights reserved.