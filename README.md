# Paradise Nursery Shopping Application

An elegant, user-friendly e-commerce web application for plant enthusiasts to explore, select, and purchase various houseplants. Developed with **React**, **Redux Toolkit**, and **Vite**.

---

## 🌿 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Components & Grading Breakdown](#components--grading-breakdown)
- [License](#license)

---

## 🪴 Overview

**Paradise Nursery** is an online plant shop application that allows users to:
1. Land on an inviting welcome page featuring the nursery mission and background imagery.
2. Browse a rich catalog of houseplants categorized into multiple collections (Air Purifying, Aromatic Fragrant, Insect Repellent, Medicinal, and Low Maintenance).
3. Add desired plants directly to a shopping cart with real-time cart badge quantity updates.
4. Manage selected items in a responsive shopping cart, including incrementing, decrementing, or removing plants with real-time subtotal and total price calculations.

---

## ✨ Features

- **Landing Page (`App.jsx` & `App.css`)**:
  - Immersive greenhouse background image.
  - Company branding: "Paradise Nursery" and tagline "Where Green Meets Serenity".
  - "Get Started" call-to-action button transitioning seamlessly to the plant catalog.
  - Informative **About Us** section describing the nursery's passion and commitment.

- **Plant Catalog (`ProductList.jsx`)**:
  - Grouped into 5 distinct categories with 6 unique plants per category (30 plants in total).
  - Each product card displays a high-quality plant thumbnail, plant name, description, and unit price.
  - Interactive "Add to Cart" button that disables and changes label to "Added to Cart" once selected.
  - Persistent navigation bar with links to Home, Plants, and Cart with live item count badge.

- **Redux State Management (`CartSlice.jsx` & `store.js`)**:
  - Centralized cart state powered by `@reduxjs/toolkit`.
  - `addItem`: Adds an item or increments its quantity if already present.
  - `removeItem`: Removes a product from the shopping cart.
  - `updateQuantity`: Updates plant item quantities dynamically.

- **Shopping Cart Experience (`CartItem.jsx`)**:
  - Itemized overview showing thumbnail, plant name, unit price, quantity controls, and plant subtotal.
  - Increase (`+`) and decrease (`-`) quantity buttons with automatic removal when count reaches zero.
  - Delete button to immediately remove items.
  - Dynamic overall cart total amount.
  - "Continue Shopping" button returning back to the product listing.
  - "Checkout" button providing a "Coming Soon" notification.

---

## 📂 Project Structure

```text
paradise-nursery-react-app/
├── public/
│   └── vite.svg
├── src/
│   ├── assets/
│   ├── AboutUs.css
│   ├── AboutUs.jsx
│   ├── App.css
│   ├── App.jsx
│   ├── CartItem.css
│   ├── CartItem.jsx
│   ├── CartSlice.jsx
│   ├── index.css
│   ├── main.jsx
│   ├── ProductList.css
│   ├── ProductList.jsx
│   └── store.js
├── index.html
├── package.json
├── README.md
└── vite.config.js
```

---

## 🛠️ Technologies Used

- **React 18**: UI component library
- **Redux Toolkit**: Predictable global state management
- **React-Redux**: Official React bindings for Redux
- **Vite**: Ultra-fast frontend build tool and dev server
- **CSS3**: Responsive flexbox and grid styling

---

## 🚀 Getting Started

### Prerequisites

- Node.js (version 16 or later)
- npm or yarn

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/Harshjoshi211/paradise-nursery-react-app.git
   cd paradise-nursery-react-app
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the local development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to the displayed localhost URL (typically `http://localhost:5173/`).

---

## 📝 Components & Grading Breakdown

| Task | File | Description |
|---|---|---|
| **Task 1** | `README.md` | Project name, details, features, and setup instructions. |
| **Task 2** | `src/AboutUs.jsx` | Company details, mission statement, and background. |
| **Task 3** | `src/App.css` | Landing page styling and background image implementation. |
| **Task 4** | `src/App.jsx` | Landing page with company name and "Get Started" button. |
| **Task 5** | `src/CartSlice.jsx` | Redux slice with `addItem`, `removeItem`, and `updateQuantity`. |
| **Task 6** | `src/ProductList.jsx` | Categorized plant catalog, Add to Cart handling, navbar, and cart counter. |
| **Task 7** | `src/CartItem.jsx` | Cart page, item total and cart total calculations, quantity adjustment, continue shopping, and checkout. |

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.