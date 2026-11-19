# Inventory & Data Management System

Setup: `npm install`, copy `.env.example` to `.env`, start MongoDB, then `npm start`.

| Method | Endpoint | Purpose |
|---|---|---|
| POST | /api/products | Create product |
| GET | /api/products | List (category, supplier, search, minPrice, maxPrice, inStock, sort, page, limit) |
| GET | /api/products/:id | Single product |
| PUT | /api/products/:id | Update details |
| PATCH | /api/products/:id/stock | `{ "change": 10 }` restock, `{ "change": -3 }` sale |
| DELETE | /api/products/:id | Delete |
| GET | /api/products/low-stock | quantity <= reorderLevel |
| GET | /api/products/summary | Category-wise aggregation |

Example: `GET /api/products?category=Furniture&sort=-price&page=1&limit=5`



## Project Features

- Product creation and management
- Product search and filtering
- Sorting and pagination
- Product details update
- Stock adjustment
- Low-stock report
- Category-wise inventory summary
- Input validation and error handling

## Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- dotenv
- Postman

## Installation

1. Clone the repository.
2. Run `npm install`.
3. Create a `.env` file using `.env.example`.
4. Start MongoDB.
5. Run `npm start`.

Server URL: `http://localhost:5000`

## API Testing

All implemented API endpoints were tested using Postman.

## Postman Screenshots

## API Screenshots

### 1. Get All Products
![Get All Products](screenshots/get-all-products.png)

## Author

Krish Singh Randhawa


