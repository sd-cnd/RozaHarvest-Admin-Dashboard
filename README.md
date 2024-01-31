# RozaHarvest Admin Dashboard

[![RozaHarvest Admin Dashboard](https://i.postimg.cc/HkR459nT/Roza-Dashboard.png)](https://roza-harvest-admin-dashboard.vercel.app/)

## Overview

Welcome to the RozaHarvest Admin Dashboard, a powerful e-commerce management tool developed using TypeScript, Next.js, and Tailwind CSS. This dashboard is designed to provide seamless control over multiple vendors and stores through a unified CMS. With features like dynamic product management, filter customization, and comprehensive sales tracking, RozaHarvest Admin Dashboard empowers you to take charge of your e-commerce ecosystem.

## Technologies Used

- **Languages:** TypeScript
- **Frameworks:** Next.js
- **Styling:** Tailwind CSS
- **Authentication:** Clerk
- **Database:** Supabase (PostgreSQL)
- **ORM:** Prisma
- **UI Libraries:** Shadcn/UI
- **Deployment:** Vercel
- **Additional Tools:** Stripe

## Key Features

- **Admin Dashboard as CMS and API:**
  - Manage multiple vendors and stores through a single CMS.
  - Generate API routes for individual stores (e.g., "Shoe store," "Laptop store").

- **Category and Product Management:**
  - Create, update, and delete categories.
  - Create, update, and delete products.
  - Upload multiple images for products and modify them dynamically.

- **Filter Management:**
  - Create, update, and delete filters (e.g., "Color," "Size").
  - Associate filters with product creation for seamless matching.

- **Billboard Management:**
  - Create, update, and delete billboards.
  - Attach billboards to a single category or use them standalone.

- **Search and Pagination:**
  - Search through categories, products, sizes, colors, and billboards.
  - Pagination for enhanced navigation.

- **Featured Products:**
  - Control which products are "featured" for display on the homepage.

- **Order and Sales Tracking:**
  - Monitor orders, sales, and revenue.
  - Graphical representation of revenue trends.

- **Authentication and Checkout:**
  - Implement Clerk Authentication.
  - Order creation and Stripe checkout.
  - Handle Stripe webhooks for secure transactions.

## Prerequisites

Ensure you have Node.js version 14.x installed.

## Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/sd-cnd/RozaHarvest-Admin-Dashboard.git

### Setup .env file


```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# This was inserted by `prisma init`:
# Environment variables declared in this file are automatically made available to Prisma.
# See the documentation for more detail: https://pris.ly/d/prisma-schema#accessing-environment-variables-from-the-schema

# Prisma supports the native connection string format for PostgreSQL, MySQL, SQLite, SQL Server, MongoDB and CockroachDB.
# See the documentation for all the connection string options: https://pris.ly/d/connection-strings

DATABASE_URL=''
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=""
STRIPE_API_KEY=
FRONTEND_STORE_URL=http://localhost:3001
STRIPE_WEBHOOK_SECRET=
```

### Connect to Supabase and Push Prisma
```shell
npx prisma generate
npx prisma db push
```


### Start the app

```shell
npm run dev
```

## Available commands

Running commands with npm `npm run [command]`

| command         | description                              |
| :-------------- | :--------------------------------------- |
| `dev`           | Starts a development instance of the app |


