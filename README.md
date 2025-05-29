# UrbanDrobe-Your Wardrobe Upgrade Starts Here!

This is a modern e-commerce frontend application built with **React** and **Redux Toolkit** for state management. The app allows users to browse products, add or remove items from the cart, and proceed through a checkout process with a billing form. It also includes a simple contact page.

---

## Live Demo

[Click Here](https://urban-drobe-your-wardrobe-upgrade-s.vercel.app/)

---

## Features

- **Product Listing**: Display of products with add-to-cart functionality.
- **Shopping Cart**: Add items to the cart, update quantities, or remove items.
- **Cart Persistence**: Cart state is saved and loaded from `localStorage` to persist user choices across sessions.
- **Checkout Page**: Shows order summary, billing address form, and payment form (form submission disabled).
- **Contact Page**: Basic contact form (submission disabled).
- **Redux Toolkit**: Used for managing cart state efficiently.
- **React Router**: For navigation between Home, Checkout, and Contact pages.
- **Bootstrap & Custom Styling**: Responsive UI with Bootstrap classes and custom styles.
- **Navbar & Footer**: Shared components across all pages.

---

## Project Structure
```bash
- `/components` – Reusable components like `Navbar`, `Footer`, `Main`, and `Product`.
- `/pages` – Main pages including `Home.js`, `Checkout.js`, and `ContactPage.js`.
- `/redux` – Redux setup including reducers (`handleCart`), root reducer, and store configuration.
- `/App.js` – App routing and page rendering.
- `/fakeAPI.js` (conceptual) – Used as a mock API or simulated backend for product data during development (highlighted below).
```
----

## Key Highlights

### 1. **Redux Cart Reducer (`handleCart`)**

- Adds items to cart, increments quantity if the item exists.
- Deletes or decrements item quantity.
- Saves updated cart to `localStorage` for persistence.
- Handles empty cart scenario gracefully.

### 2. **Checkout Page**

- Displays order summary with total price and shipping.
- Billing address form with validation UI (but submission is disabled for now).
- Payment details form (submission disabled).

### 3. **fakeAPI (Mock API Concept)**

> **Note:** The project uses a **fakeAPI** or mock API to simulate backend calls and product data during development. This approach allows frontend development and testing without a real backend service.

- Typically, `fakeAPI` is a JS module or JSON file exporting product data arrays.
- Can be extended to simulate async calls using `setTimeout` or Promises.
- Useful for prototyping UI and Redux store integration before real API integration.

---

## Installation

```bash
git clone https://github.com/KavanaBC/UrbanDrobe_Your-Wardrobe-Upgrade-Starts-Here.git
cd urbandrobe
npm install
npm start
```
---
