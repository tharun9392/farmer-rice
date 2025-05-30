﻿# FarmeRice - Rice Farming and Trading Platform

FarmeRice is a comprehensive MERN stack application that connects farmers, customers, and administrators in a rice trading ecosystem. The platform facilitates rice trading, inventory management, and farmer-customer interactions.

## 🌾 Features

### For Customers
- Browse and purchase rice products
- Track orders in real-time
- Manage shopping cart
- Submit product reviews
- Secure payment processing
- Order history and tracking
- Profile management

### For Farmers
- List rice products for sale
- Manage inventory
- Track sales and transactions
- Communicate with customers
- View analytics and reports
- Manage product listings

### For Administrators
- User management
- Inventory forecasting
- Order analytics
- Staff management
- Task assignment
- Product approval
- System monitoring

## 🚀 Technology Stack

### Backend
- Node.js (≥18.0.0)
- Express.js
- MongoDB with Mongoose
- JWT Authentication
- SendGrid for emails
- Razorpay for payments
- Winston for logging

### Frontend
- React 18
- Redux Toolkit
- React Router
- Tailwind CSS
- Formik & Yup
- Axios
- Recharts

## 📦 Installation

### Prerequisites
- Node.js ≥18.0.0
- MongoDB
- npm or yarn
- Git

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd Farm-Backend-main
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `config.env` file in the root directory with the following variables:
   ```env
   NODE_ENV=development
   PORT=5015
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   JWT_EXPIRE=30d
   SENDGRID_API_KEY=your_sendgrid_api_key
   RAZORPAY_KEY_ID=your_razorpay_key_id
   RAZORPAY_KEY_SECRET=your_razorpay_key_secret
   FRONTEND_URL=http://localhost:3000
   ```

4. Start the backend server:
   ```bash
   npm run dev
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd farm_frontend-main
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory:
   ```env
   REACT_APP_API_URL=http://localhost:5015/api
   REACT_APP_RAZORPAY_KEY_ID=your_razorpay_key_id
   ```

4. Start the frontend development server:
   ```bash
   npm start
   ```

## 🌐 Usage

### Accessing the Application
- Frontend: http://localhost:3000
- Backend API: http://localhost:5015

### User Roles
1. **Customer**
   - Register/Login
   - Browse products
   - Place orders
   - Track deliveries

2. **Farmer**
   - Manage products
   - Track sales
   - Communicate with customers
   - View analytics

3. **Administrator**
   - Manage users
   - Monitor transactions
   - Generate reports
   - System configuration

## 🔒 Security Features
- JWT Authentication
- Password encryption
- Input sanitization
- XSS protection
- Rate limiting
- Secure headers
- CORS configuration

## 📊 API Documentation

### Authentication Endpoints
- POST /api/auth/register - Register new user
- POST /api/auth/login - User login
- POST /api/auth/forgot-password - Password recovery
- POST /api/auth/reset-password - Reset password

### Product Endpoints
- GET /api/products - List all products
- POST /api/products - Create new product
- GET /api/products/:id - Get product details
- PUT /api/products/:id - Update product
- DELETE /api/products/:id - Delete product

### Order Endpoints
- POST /api/orders - Create order
- GET /api/orders - List user orders
- GET /api/orders/:id - Get order details
- PUT /api/orders/:id - Update order status

### User Endpoints
- GET /api/users/profile - Get user profile
- PUT /api/users/profile - Update profile
- GET /api/users - List all users (admin)
- PUT /api/users/:id - Update user (admin)

## 🛠️ Development

### Running Tests
```bash
# Backend tests
cd Farm-Backend-main
npm test

# Frontend tests
cd farm_frontend-main
npm test
```

### Building for Production
```bash
# Backend
cd Farm-Backend-main
npm run build

# Frontend
cd farm_frontend-main
npm run build
```

## 🤝 Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 👥 Authors
- Initial work - [tharun9392](https://github.com/tharun9392)

## 🙏 Acknowledgments
- Node.js community
- React community
- MongoDB team
- All contributors and supporters
# farmer-rice
