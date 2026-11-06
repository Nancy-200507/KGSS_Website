
# GreenCart – Online Grocery Shopping Platform

GreenCart is a full-stack online grocery shopping platform built using the MERN stack. It provides customers with a convenient way to browse grocery products, manage their shopping cart, place orders, and track purchases. It also includes a seller dashboard for managing products and customer orders.

## Features

### Customer Features
- User registration and login.
- Browse grocery products and categories.
- View product details and pricing.
- Add products to the shopping cart.
- Update product quantities and manage cart items.
- Save and manage delivery addresses.
- Place Cash on Delivery (COD) orders.
- View order history.

### Seller Features
- Secure seller authentication.
- Add new products with images and descriptions.
- Manage product listings.
- Update product stock availability.
- View customer orders.
- Manage order-related information.

## Tech Stack

Frontend:
- React.js
- Vite
- Tailwind CSS
- React Router
- Axios

Backend:
- Node.js
- Express.js

Database:
- MongoDB
- Mongoose

Authentication & Security:
- JSON Web Tokens (JWT)
- bcrypt
- HTTP-only Cookies

Other Tools & Integrations:
- Cloudinary (Image Storage)
- React Hot Toast (Notifications)
- Stripe (Payment Integration – backend implementation)

## Project Structure

text
GreenCart/
│
├── client/
│   ├── public/
│   └── src/
│       ├── assets/
│       ├── components/
│       ├── context/
│       └── pages/
│           └── seller/
│
└── server/
    ├── configs/
    ├── controllers/
    ├── middlewares/
    ├── models/
    └── routes/


## Installation and Setup

### Prerequisites
- Node.js
- npm
- MongoDB
- Cloudinary Account

### 1. Clone the Repository

bash
git clone https://github.com/Nancy-200507/KGSS_Website.git
cd KGSS_Website/greencart-main


### 2. Backend Setup

bash
cd server
npm install


Create a `.env` file inside the server directory:

env
PORT=8000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

SELLER_EMAIL=your_seller_email
SELLER_PASSWORD=your_seller_password

STRIPE_SECRET_KEY=your_stripe_secret_key


Start the backend server:

bash
npm start


Backend runs at:

text
http://localhost:8000


### 3. Frontend Setup

Open another terminal:

bash
cd client
npm install


Create a `.env` file inside the client directory:

env
VITE_BACKEND_URL=http://localhost:8000
VITE_CURRENCY=$


Start the frontend:

bash
npm run dev


Frontend runs at:

text
http://localhost:5173


## API Routes

| Route | Description |
|---|---|
| `/api/user` | User authentication and account management |
| `/api/seller` | Seller authentication |
| `/api/product` | Product management |
| `/api/cart` | Shopping cart operations |
| `/api/address` | Delivery address management |
| `/api/order` | Order placement and order retrieval |

## Future Improvements

- Integrate live product data from MongoDB into the storefront.
- Complete and enable Stripe payment processing and webhook handling.
- Implement automated frontend and backend testing.
- Improve error handling and input validation.
- Enhance the user experience and add more shopping features.

## Author

Sahagya Nancy Maruthuvar

GitHub: [Nancy-200507](https://github.com/Nancy-200507)

