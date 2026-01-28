# 🛒 E-Commerce Backend API

This is the backend server for an **E-Commerce Website** built using **Node.js, Express.js, MongoDB, and JWT authentication**.  
It provides REST APIs for product management, user authentication, cart handling, and image uploads.  
An **Admin Panel** consumes these APIs to add, update, and manage products on the platform.

---

## 🚀 Tech Stack

- **Node.js**
- **Express.js**
- **MongoDB (Mongoose)**
- **JWT (JSON Web Token)** – Authentication
- **Multer** – Image Uploads
- **CORS**
- **dotenv**

---

## 📌 Features

### 👤 User Features
- User Registration (Signup)
- User Login with JWT Authentication
- Add products to cart
- Remove products from cart
- Fetch cart data

### 🛍️ Product Features
- Add new products (Admin)
- Remove products (Admin)
- Fetch all products
- Fetch new collections
- Fetch popular products (Women category)
- Image upload support for products

### 🧑‍💼 Admin Panel
- Add products with images
- Update product listings
- Manage product availability

---

## 📂 Project Structure
```
backend/
│
├── upload/
│ └── images/ # Uploaded product images
│
├── index.js # Main server file
├── .env # Environment variables
├── package.json
└── README.md
```
---

## ⚙️ Environment Variables

Create a `.env` file in the root directory and add the following:

```env
PORT=4000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
```
## 🔧 Installation & Setup

Clone the repository
```

git clone https://github.com/your-username/ecommerce-backend.git
```

Navigate to the project directory
```
cd ecommerce-backend

```
Install dependencies
```
npm install

```
Run the server
```
npm start
```

Server will run at:
```
http://localhost:4000
```
---
## 📡 API Endpoints
| Method | Endpoint  | Description       |
| ------ | --------- | ----------------- |
| POST   | `/signup` | Register new user |
| POST   | `/login`  | Login user        |

## 📦 Products

| Method | Endpoint          | Description            |
| ------ | ----------------- | ---------------------- |
| POST   | `/addproduct`     | Add new product        |
| POST   | `/removeproduct`  | Remove product         |
| GET    | `/allproducts`    | Get all products       |
| GET    | `/newcollections` | Latest products        |
| GET    | `/popularinwomen` | Popular women products |

## 🛒 Cart

| Method | Endpoint          | Description           |
| ------ | ----------------- | --------------------- |
| POST   | `/addtocart`      | Add item to cart      |
| POST   | `/removefromcart` | Remove item from cart |
| POST   | `/getcart`        | Get cart data         |

## 🔑 Authentication

- JWT is used for secure authentication

- Token must be sent in request headers as:

- auth-token: <JWT_TOKEN>

## 🧩 Frontend Integration

This backend is designed to work with a React.js frontend.
The frontend consumes APIs for:
- User login & registration
- Product listing
- Cart management
- Admin panel operations

## 📌 Future Improvements
- Password hashing with bcrypt
- Role-based authentication (Admin/User)
- Product update API
- Order & payment integration
- Pagination & filtering

👨‍💻 Author

Built as part of a Full Stack E-Commerce Project using
Express, Node.js, MongoDB, and React.js
