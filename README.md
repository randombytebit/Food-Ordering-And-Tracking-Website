<div align="center">

# Food Ordering and Tracking Website

**A full-stack website for browsing restaurants, placing orders, and tracking deliveries in real-time.**

[![React](https://img.shields.io/badge/React-18.x-61DAFB?style=flat-square&logo=react&logoColor=white)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Express](https://img.shields.io/badge/Express-4.x-000000?style=flat-square&logo=express&logoColor=white)](https://expressjs.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-7.x-47A248?style=flat-square&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Auth0](https://img.shields.io/badge/Auth0-Enabled-EB5424?style=flat-square&logo=auth0&logoColor=white)](https://auth0.com/)

[Live Demo](https://github.com/Shiro12222/Shiro12222-Food-Ordering-And-Tracking-App) · [Report Bug](https://github.com/Shiro12222/Shiro12222-Food-Ordering-And-Tracking-App/issues) · [Request Feature](https://github.com/Shiro12222/Shiro12222-Food-Ordering-And-Tracking-App/issues)

</div>

---

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Running Tests](#running-tests)
- [Contributing](#contributing)

---

## About the Project

The Food Ordering and Tracking App is designed to streamline the end-to-end food ordering experience. Users can browse restaurant listings, explore menus, place orders, complete payments, and monitor delivery status in real-time. The platform supports both guest and authenticated users, and provides restaurant operators with tools to manage their operations effectively.

---

## Features

| Category | Description |
|---|---|
| **User Authentication** | Secure login and registration via Auth0, supporting both guest and authenticated sessions |
| **Restaurant Browsing** | Explore restaurants with filtering by district, cuisine type, and ratings |
| **Menu Viewing** | Browse detailed menus per restaurant with item descriptions and pricing |
| **Order Management** | Streamlined checkout flow with real-time order status tracking |
| **Profile Management** | Users can update personal details and preferences |

---

## Tech Stack

**Frontend**

| Technology | Purpose |
|---|---|
| [React](https://reactjs.org/) | UI component framework |
| [TypeScript](https://www.typescriptlang.org/) | Type-safe JavaScript |
| [Tailwind CSS](https://tailwindcss.com/) | Utility-first styling |
| [shadcn/ui](https://ui.shadcn.com/) | Accessible UI component library |

**Backend**

| Technology | Purpose |
|---|---|
| [Express.js](https://expressjs.com/) | REST API server |
| [MongoDB](https://www.mongodb.com/) | NoSQL database |

**Tools & Services**

| Tool | Purpose |
|---|---|
| [Auth0](https://auth0.com/) | Authentication and authorization |
| [Mocha](https://mochajs.org/) | Unit testing framework |

---

## Project Structure

```
food-ordering-and-tracking-app/
├── food-ordering-and-tracking-app-frontend/
│   ├── src/
│   │   ├── components/         # Reusable UI components
│   │   ├── pages/              # Route-level page components
│   │   ├── hooks/              # Custom React hooks
│   │   ├── types/              # TypeScript type definitions
│   │   └── main.tsx            # Application entry point
│   ├── public/
│   ├── tailwind.config.ts
│   ├── tsconfig.json
│   └── package.json
│
└── food-ordering-and-tracking-app-backend/
    ├── src/
    │   ├── models/             # Mongoose data models
    │   ├── routes/             # Express route handlers
    │   ├── middleware/         # Auth and validation middleware
    │   └── index.ts            # Server entry point
    ├── test/                   # Mocha unit tests
    └── package.json
```

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v18 or higher
- [npm](https://www.npmjs.com/) v9 or higher
- A [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) cluster
- An [Auth0](https://auth0.com/) account and application

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/randombytebit/Food-Ordering-And-Tracking-Website.git
   ```

2. **Install frontend dependencies**

   ```bash
   cd frontend
   npm install
   ```

3. **Configure frontend environment variables**

   Create a `.env` file in the frontend directory:

   ```env
   VITE_AUTH0_DOMAIN=your_auth0_domain
   VITE_AUTH0_CLIENT_ID=your_auth0_client_id
   VITE_API_BASE_URL=http://localhost:7000
   ```

4. **Install backend dependencies**

   ```bash
   cd ..
   cd backend
   npm install
   ```

5. **Configure backend environment variables**

   Create a `.env` file in the backend directory:

   ```env
   MONGODB_URL=your_mongodb_connection_string
   AUTH0_AUDIENCE=your_auth0_api_audience
   AUTH0_ISSUER_BASE_URL=https://your_auth0_domain
   PORT=7000
   ```

### Running the Application

Start both servers in separate terminal windows.

**Backend**

```bash
cd backend
npm run dev
```

**Frontend**

```bash
cd frontend
npm run dev
```

The frontend will be available at [http://localhost:5173](http://localhost:5173) and the backend API at [http://localhost:7000](http://localhost:7000).

---

## Running Tests

Unit tests are written using [Mocha](https://mochajs.org/) and located in the backend `test/` directory.

```bash
cd backend
npm test
```

---

## Contributing

Contributions are welcome. To propose a change:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature-name`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature-name`)
5. Open a Pull Request

---

<div align="center">

Food Ordering and Tracking App · Built with React, Express, and MongoDB

</div>
