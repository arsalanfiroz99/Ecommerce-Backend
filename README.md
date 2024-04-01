
# NodeJs: Build The Complete E-Commerce Web API

---

## Installation and Setup

To set up and run this ecommerce backend locally, follow these steps:

### Install Dependencies

```bash
npm install
```

This command installs all the necessary npm packages as defined in `package.json`.

### Start the API

```bash
npm start
```

This command starts the Node.js application, and the API will be accessible on `http://localhost:3000` by default.

## API Routes Overview

The backend provides a structured set of RESTful API endpoints categorized by resources such as Products, Orders, and Users. Each category supports standard CRUD operations and additional functionalities:

### Products

- **List all products**: `GET /api/v1/products`
- **Retrieve a single product by ID**: `GET /api/v1/products/:id`
- **Add a new product** (Admin only): `POST /api/v1/products`
- **Update a product by ID** (Admin only): `PUT /api/v1/products/:id`
- **Delete a product by ID** (Admin only): `DELETE /api/v1/products/:id`
- **Update product gallery images**: `PUT /api/v1/products/gallery-images/:id`
- **Get featured products**: `GET /api/v1/products/get/featured/:count`
- **Get total products count**: `GET /api/v1/products/get/count`

### Orders

- **List all orders**: `GET /api/v1/orders`
- **Retrieve a single order by ID**: `GET /api/v1/orders/:id`
- **Create a new order**: `POST /api/v1/orders`
- **Update an order by ID**: `PUT /api/v1/orders/:id`
- **Delete an order by ID**: `DELETE /api/v1/orders/:id`
- **Get total orders count**: `GET /api/v1/orders/get/count`

### Users

- **List all users**: `GET /api/v1/users`
- **Retrieve a single user by ID**: `GET /api/v1/users/:id`
- **Add a new user**: `POST /api/v1/users`
- **Update a user by ID**: `PUT /api/v1/users/:id`
- **Delete a user by ID**: `DELETE /api/v1/users/:id`
- **Get total users count**: `GET /api/v1/users/get/count`
- **Register a new user**: `POST /api/v1/users/register`
- **User login**: `POST /api/v1/users/login`

## Key Features

- Scalable backend with Node.js, supporting secure authentication and dynamic management of products and orders.
- Comprehensive RESTful API endpoints crafted with Express.js for frontend integration, CRUD operations, and additional features like image galleries and featured products.
- Secure endpoint access with JWT, ensuring data integrity and admin-only privileges for critical product and order operations.
- Advanced order management features, including analytics on total sales and personalized user order histories, enhancing operational efficiency and user experience.
- Robust error handling and validation with middleware, ensuring API reliability.
