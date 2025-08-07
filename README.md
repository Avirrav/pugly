# Full Stack E-Commerce + Dashboard & CMS

## Technologies Used:
- **Next.js 13 App Router**
- **React**
- **Tailwind CSS**
- **Prisma & PostgreSQL **
- **Shadcn UI (Admin Panel)**
- **AWS EC2 (Hosting)**
- **Clerk Authentication**
- **Razorpay (Payments & Webhooks)**

## Overview
This repository contains a full-stack eCommerce platform with an integrated admin dashboard serving as both a CMS and API. It allows management of multiple vendors/stores and provides extensive control over categories, products, and order tracking.

## Key Features
### **Admin Dashboard (CMS & API)**
- **Multi-Vendor Support**: Manage multiple stores (e.g., Shoe Store, Laptop Store, Suit Store) with dynamically generated API routes.
- **Category Management**: Create, update, and delete product categories.
- **Product Management**: Create, update, and delete products.
- **Image Uploads**: Upload multiple images for products and update them anytime.
- **Filters & Variations**: Define and manage attributes like "Color" and "Size".
- **Billboards**: Manage large promotional texts, attachable to categories or standalone.
- **Search & Pagination**: Search through categories, products, sizes, colors, and billboards with pagination.
- **Featured Products**: Highlight specific products on the homepage.
- **Sales & Orders Tracking**: View orders, sales metrics, and analytics.
- **Revenue Graphs**: Visualize revenue trends.



## Prerequisites
- **Node.js** (Version 14.x or higher)
- **PostgreSQL Database**

## Installation & Setup
### 1. **Clone the Repository**
```bash
git clone https://github.com/Avirrav/pugly
```
### 2. **Install Dependencies**
```bash
npm install
```

### 3. **Setup Environment Variables**
Create a `.env` file in the root directory and add the following:
```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/
DATABASE_URL=""
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=''
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
FRONTEND_STORE_URL=http://localhost:3001
```

### 4. **Connect to Database & Apply Migrations**
```bash
npx prisma generate
npx prisma db push
```

### 5. **Start the Application**
```bash
npm run dev
```

## Available Commands
| Command | Description |
|---------|-------------|
| `npm run dev` | Starts the development server |

This project is designed to be scalable and easily customizable for different eCommerce business needs. 🚀

