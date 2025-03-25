# MERN E-Commerce 2024

Welcome to this MERN e-commerce project, which let you build an online store with a React frontend and Node/Express/MongoDB backend. While there might be some grammar mistakes, this doc is meant to be helpful and clarity the project structure.

## Overview
This repository is splitted into two parts:
1. **Server** folder for Node.js backend with Express.
2. **Client** folder for React-based frontend.

## Project Structure
## Backend (Server)
- **server.js** sets up the Express app, connects to MongoDB, and defines routes.
- **models** holds Mongoose schemas (e.g. `User.js`, `Product.js`, `Order.js`).
- **controllers** contains request handlers for things like auth, shop, or admin tasks.
- **routes** organizes all API endpoints, such as `/api/shop/cart` or `/api/admin/products`.

### Key Points
- Uses **JWT** for authentication (`auth-controller.js` demonstrates login, register, logout).
- Provides various endpoints for listing, creating, & editing products in admin scope.
- Payment integration with `paypal.js`.
- **CORS** is configured to allow `http://localhost:5173` for dev environment.

## Frontend (Client)
- Built with **React** + **Vite** for fast dev server and bundling.
- **`src/components`** folder has reusable UI and layout components (e.g. `AuthLayout`, `AdminLayout`).
- **`src/pages`** holds page-specific modules like `login` or admin pages (`admin-view`, `shopping-view`).
- Global state management is done with **Redux Toolkit** (see `store` folder).
- Routing uses **React Router** (defined in `App.jsx`).

### Key Points
- The user’s authentication state is tracked in Redux and synced from the backend with cookies.
- Contains pages for registration, login, product listing, cart, order checkout, etc.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/mern-ecommerce-2024.git
## Backend (Server)
- **server.js** sets up the Express app, connects to MongoDB, and defines routes.
- **models** holds Mongoose schemas (e.g. `User.js`, `Product.js`, `Order.js`).
- **controllers** contains request handlers for things like auth, shop, or admin tasks.
- **routes** organizes all API endpoints, such as `/api/shop/cart` or `/api/admin/products`.

### Key Points
- Uses **JWT** for authentication (`auth-controller.js` demonstrates login, register, logout).
- Provides various endpoints for listing, creating, & editing products in admin scope.
- Payment integration with `paypal.js`.
- **CORS** is configured to allow `http://localhost:5173` for dev environment.

## Frontend (Client)
- Built with **React** + **Vite** for fast dev server and bundling.
- **`src/components`** folder has reusable UI and layout components (e.g. `AuthLayout`, `AdminLayout`).
- **`src/pages`** holds page-specific modules like `login` or admin pages (`admin-view`, `shopping-view`).
- Global state management is done with **Redux Toolkit** (see `store` folder).
- Routing uses **React Router** (defined in `App.jsx`).

### Key Points
- The user’s authentication state is tracked in Redux and synced from the backend with cookies.
- Contains pages for registration, login, product listing, cart, order checkout, etc.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/mern-ecommerce-2024.git