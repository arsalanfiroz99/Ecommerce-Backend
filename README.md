# Node.js eCommerce Web API

## Introduction
This Node.js application serves as the backend for an eCommerce platform, providing a comprehensive set of RESTful API endpoints for managing products, orders, and user accounts. It supports secure authentication and offers dynamic management capabilities for products and orders.

## Key Features
- **Product Management**: Add, update, delete, and list products, including image galleries and featured product listings.
- **Order Management**: Create, update, delete, and list orders along with analytics on total sales.
- **User Management**: Register new users, user login, list, update, and delete user accounts.
- **Secure Authentication**: Utilize JWT for secure endpoint access, ensuring data integrity and restricted admin privileges.
- **Dynamic Management**: Manage products and orders with comprehensive RESTful API endpoints.
- **Error Handling**: Robust error handling and validation for reliability.

## Technologies Used
- **Node.js**: The runtime environment for running the JavaScript server.
- **Express.js**: The web application framework used for API creation.
- **MongoDB**: The database used for storing application data.
- **JWT**: Used for authentication.

## Getting Started

### Prerequisites
Ensure you have the following installed:
- Node.js
- npm (Node Package Manager)
- MongoDB

### Installation
1. **Clone the repository**:
   ```
   git clone https://github.com/<your-username>/eCommerce_Backend.git
   ```
   Replace `<your-username>` with your GitHub username or the organization/user under which the repository is hosted.

2. **Navigate to the project directory**:
   ```
   cd eCommerce_Backend
   ```

3. **Install dependencies**:
   ```
   npm install
   ```

### Running the Application
1. **Start the API**:
   ```
   npm start
   ```
   This command starts the Node.js application. The API will be accessible on `http://localhost:3000` by default.

## Usage
- **Product Operations**: Perform CRUD operations on products using the `/api/v1/products` endpoint.
- **Order Operations**: Manage orders through the `/api/v1/orders` endpoint.
- **User Operations**: Manage user accounts via the `/api/v1/users` endpoint.

For detailed endpoint documentation, refer to the API Routes Overview section.

---

This format maintains the structure and content of the original eCommerce backend README but presents it in a more organized and consistent manner, similar to the URL Shortener README.

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
  
## Contributing
Contributions to the eCommerce Web API are welcome! Feel free to fork the repository, make your improvements, and submit pull requests.
