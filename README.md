# Food-Del - Food Delivery Application

A full-stack food delivery application built with React, Node.js, and MongoDB. This project includes an admin panel for restaurant management, a customer-facing frontend, and a robust backend API.

## Project Structure

```
Food-Del/
├── admin/          # Admin dashboard for food management
├── frontend/       # Customer-facing React application
├── backend/        # Node.js REST API server
└── README.md
```

## Features

### Admin Panel
- Add, edit, and manage food items
- View order list
- Manage food inventory
- User-friendly dashboard with sidebar navigation

### Frontend
- Browse food menu by categories
- Add items to cart
- Place orders
- Track order status
- User authentication
- Download mobile app links

### Backend
- User authentication and management
- Food catalog management
- Shopping cart operations
- Order processing
- Order tracking
- Secure API endpoints

## Tech Stack

### Frontend
- **React** - UI library
- **Vite** - Build tool
- **CSS3** - Styling

### Admin
- **React** - UI library
- **Vite** - Build tool
- **CSS3** - Styling

### Backend
- **Node.js** - Runtime environment
- **Express** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM for MongoDB
- **JWT** - Authentication

## Installation

### Prerequisites
- Node.js (v14 or higher)
- MongoDB
- npm or yarn

### Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file in the backend directory:
```
PORT=4000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

Start the backend server:
```bash
npm start
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

### Admin Setup

```bash
cd admin
npm install
npm run dev
```

## Project Structure Details

### Backend Routes
- `/api/user` - User authentication and management
- `/api/food` - Food items management
- `/api/cart` - Shopping cart operations
- `/api/order` - Order management

### Database Models
- **User** - User account information
- **Food** - Food items with pricing and categories
- **Order** - Order details and status
- **Cart** - User shopping cart items

### Frontend Pages
- **Home** - Landing page with menu
- **Cart** - Shopping cart page
- **PlaceOrder** - Checkout page
- **Verify** - Order verification
- **MyOrders** - User order history

### Admin Pages
- **Add** - Add new food items
- **List** - View all food items
- **Orders** - Manage customer orders

## API Endpoints

### User Routes
- `POST /api/user/register` - Register new user
- `POST /api/user/login` - User login
- `GET /api/user/profile` - Get user profile

### Food Routes
- `GET /api/food/list` - Get all food items
- `POST /api/food/add` - Add new food (admin)
- `DELETE /api/food/:id` - Delete food item (admin)

### Cart Routes
- `POST /api/cart/add` - Add item to cart
- `GET /api/cart` - Get cart items
- `DELETE /api/cart/:id` - Remove item from cart

### Order Routes
- `POST /api/order/place` - Place new order
- `GET /api/order/list` - Get user orders
- `GET /api/order/:id` - Get order details

## Environment Variables

### Backend (.env)
```
PORT=4000
MONGODB_URI=mongodb://localhost:27017/food-del
JWT_SECRET=your_secret_key_here
NODE_ENV=development
```

## Running the Application

1. **Start MongoDB**
   ```bash
   mongod
   ```

2. **Start Backend Server**
   ```bash
   cd backend
   npm start
   ```

3. **Start Frontend**
   ```bash
   cd frontend
   npm run dev
   ```

4. **Start Admin Panel**
   ```bash
   cd admin
   npm run dev
   ```

## Build for Production

### Frontend
```bash
cd frontend
npm run build
```

### Admin
```bash
cd admin
npm run build
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Author

**KalyaRaunak**

## Support

For support, email support@fooddel.com or open an issue on GitHub.

---

**Note:** Make sure to update the MongoDB URI, JWT secret, and other configuration values before deploying to production.
