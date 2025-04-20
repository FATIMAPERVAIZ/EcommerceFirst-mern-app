# 🛍️ TimeZone Ecommerce App - Full Stack MERN Project

This is a full-featured E-commerce project for selling watches, built with the **MERN stack** (MongoDB, Express, React, Node.js). It includes both **Admin and User panels**, online payments (via Braintree), product management, category filters, cart, and authentication.

---

## 🧩 Tech Stack

- **Frontend**: React + Tailwind CSS
- **Backend**: Node.js + Express
- **Database**: MongoDB (Mongoose)
- **Authentication**: JWT
- **Payment Gateway**: Braintree
- **Deployment**: Vercel (Frontend) & Cyclic / Render / Vercel (Backend)

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/FATIMAPERVAIZ/EcommerceFirst-mern-app.git
cd EcommerceFirst-mern-app
```

---

### 2. Backend Setup

📁 Go to the `server` folder and install dependencies:

```bash
cd server
npm install
```

🗂️ Create a `.env` file in the `server` folder and add your environment variables:

```env
PORT=8080
DEV_MODE=Development mode
MONGO_URL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
BRAINTREE_MERCHANT_ID=your_braintree_merchant_id
BRAINTREE_PUBLIC_KEY=your_braintree_public_key
BRAINTREE_PRIVATE_KEY=your_braintree_private_key
```

▶️ Start the backend server:

```bash
npm start
```

---

### 3. Frontend Setup

📁 Go to the `client` folder and install dependencies:

```bash
cd client
npm install
```

🗂️ Create a `.env` file in the `client` folder and add this:

```env
REACT_APP_API=https://your-backend-deployment-url.com
```

> ⚠️ If you're testing locally, use:
> ```env
> REACT_APP_API=http://localhost:8080
> ```

▶️ Start the frontend:

```bash
npm start
```

---

## 🔐 Admin Access

By default, any registered user has:

```json
"role": 0  // normal user
```

To give a user **Admin access**:

1. Go to your MongoDB collection → `users`.
2. Find the user by email or ID.
3. Manually change the `role` from `0` to `1`.

```json
"role": 1  // admin user
```

✅ That user can now log in and access the **Admin dashboard**.

---

## 🌐 Deployment Notes

- Make sure your **frontend `.env`** file uses the deployed backend link.
- In your backend `cors` settings, allow:

```js
origin: [
  "https://your-frontend.vercel.app",
  "http://localhost:3000"
]
```

This ensures both development and deployed apps work properly.

---

## 🙌 Features

- ✅ User Registration & Login (JWT Auth)
- ✅ Role-based Admin Panel
- ✅ Add/Edit/Delete Categories & Products (Admin)
- ✅ Product Filtering by Category & Price
- ✅ Shopping Cart & Checkout (Braintree)
- ✅ Order Management
- ✅ Responsive UI

---

## 📸 Screenshots 
**Admin Dashboard**
![image](https://github.com/user-attachments/assets/ff00331c-e62e-43b1-8050-238a423ef35e)



## ✨ Credits

Developed by Fatima
