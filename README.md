# FullStack Portfolio Demo

A small but complete **full-stack inventory and admin dashboard** built with Node.js, Express, MySQL, HTML, CSS, and vanilla JavaScript.

The goal of this repository is to demonstrate general business-software development skills outside of game-server projects.

## What It Demonstrates

- Full-stack application structure
- REST API design
- MySQL CRUD operations
- Parameterized SQL queries
- Environment-based configuration
- Frontend API consumption
- Responsive admin dashboard UI
- Inventory statistics
- Form handling
- Error handling
- Static frontend hosting from Express

## Features

- Product inventory dashboard
- Product listing
- Add products
- Delete products
- Product detail API
- Update product API
- Inventory totals
- Low-stock counts
- Inventory value calculation
- API health endpoint

## Technology

- Node.js
- Express
- MySQL / mysql2
- JavaScript
- HTML5
- CSS3
- REST APIs
- dotenv
- CORS

## Project Structure

```text
FullStack-Portfolio-Demo/
├── public/
│   ├── app.js
│   ├── index.html
│   └── styles.css
├── src/
│   ├── routes/
│   │   ├── dashboard.js
│   │   └── products.js
│   ├── db.js
│   └── server.js
├── sql/
│   └── schema.sql
├── .env.example
├── .gitignore
├── package.json
└── README.md
```

## API Endpoints

| Method | Endpoint | Description |
| --- | --- | --- |
| GET | `/api/status` | Application health |
| GET | `/api/dashboard` | Inventory summary |
| GET | `/api/products` | List all products |
| GET | `/api/products/:id` | Get one product |
| POST | `/api/products` | Create a product |
| PUT | `/api/products/:id` | Update a product |
| DELETE | `/api/products/:id` | Delete a product |

## Setup

### 1. Install dependencies

```bash
npm install
```

### 2. Create the database

Import:

```text
sql/schema.sql
```

### 3. Configure environment variables

Copy:

```text
.env.example
```

to:

```text
.env
```

Then configure your local MySQL credentials.

### 4. Start the application

```bash
npm start
```

Open:

```text
http://localhost:3000
```

## Why This Project Exists

Much of my development work involves game systems, server platforms, launchers, APIs, and Linux infrastructure.

This project demonstrates that the same backend, database, and frontend skills also apply to traditional business applications such as:

- Inventory systems
- Admin dashboards
- Internal tools
- Product management
- Customer portals
- Operations software

## Security Notes

- Database credentials are stored in environment variables.
- `.env` is excluded from Git.
- SQL queries use parameterized values.
- Duplicate SKU errors are handled by the API.
- The example application does not include authentication and should not be exposed publicly as an admin system without adding access control.

## Author

**William Murphy / CraftEarth**

GitHub: https://github.com/CraftEarth
