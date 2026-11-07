# Porto's Bakery & Cafe — Menu Demo

A responsive, interactive bakery menu website built with **HTML, CSS, and vanilla JavaScript**. This fan-made front-end practice project recreates the feel of an online bakery menu and demonstrates client-side search, category filtering, and a demo shopping cart.

> **Disclaimer:** This is an unofficial, fan-made portfolio project created for educational purposes. It is not affiliated with, endorsed by, or an official website of Porto’s Bakery & Cafe. Menu items, descriptions, prices, and ordering interactions are illustrative only. No real orders can be placed.

## Preview

Open `portos_menu_clone.html` in a web browser to view the project locally. If you publish it using GitHub Pages, you can add your live URL here:

**Live Demo:** _Add your deployed URL here_

## Features

- **Responsive layout:** Menu cards and navigation adapt to desktop, tablet, and mobile screen sizes.
- **Menu search:** Search menu items by name, category, or description.
- **Category filters:** Browse all items, customer favorites, savory items, sweets, desserts, drinks, cakes, breakfast items, and bakery boxes.
- **Interactive demo cart:** Add menu items to an order and see the item count, quantities, line totals, and estimated total update.
- **Feedback notifications:** Toast messages confirm when an item is added and explain that checkout is only a demo.
- **Product cards:** Each menu item includes an image, category/tag, description, and illustrative price.
- **Responsive image handling:** Menu images load lazily, with a fallback background if an image fails to load.
- **Accessible interface details:** Includes labels for search and navigation, descriptive image alt text, and status messaging for cart updates.

## Technologies Used

- **HTML5** — Structures the page, navigation, menu cards, cart panel, and footer.
- **CSS3** — Provides the visual design, color variables, responsive grid layouts, hover effects, and mobile breakpoints.
- **Vanilla JavaScript** — Stores the menu data, renders category buttons and product cards, filters search results, manages cart quantities, calculates totals, and displays notifications.
- **Unsplash image URLs** — Supplies illustrative food photography for the demo.

This project does not currently require a JavaScript framework, package manager, build step, backend, or database.

## Getting Started

### Requirements

- A modern web browser
- A code editor such as Visual Studio Code (optional)

### Run locally

1. Download or clone this repository.
2. Open the project folder.
3. Open `portos_menu_clone.html` in your browser.

Alternatively, in Visual Studio Code, open the folder and use a local-server extension such as **Live Server** to preview the page.

No `npm install` or build command is needed for the current single-file version.

## How It Works

### Menu data

The `products` array in the JavaScript section contains the menu's illustrative product records. Each item includes an ID, name, category, price, tag, description, and image URL. The page generates the menu cards from this data.

### Category filtering and search

The category buttons are generated from the `categories` array. Selecting a category updates the active filter and re-renders the menu. The search field filters the visible products by their name, category, and description. Both filters can be used together.

### Demo cart

The `cart` object tracks quantities using each product's ID. When an **Add** button is clicked, the quantity increases, the cart count and line totals are recalculated, and a confirmation message appears. The estimated total is calculated in the browser from the illustrative prices.

### Checkout

Checkout is intentionally non-functional. Selecting **Continue (demo only)** displays a message confirming that no order was placed. The project has no payment processing, order submission, user accounts, or connection to Porto’s systems.

## Project Structure

The current project is a single HTML file with the styling and JavaScript included inline:

```text
portos-menu-demo/
└── portos_menu_clone.html
```

A `README.md` can be added at the repository root to document the project.

## Known Limitations

- Menu items, descriptions, prices, and product imagery are illustrative and may not match Porto’s current offerings.
- Product images are loaded from external Unsplash URLs, so an internet connection may be needed to display them.
- Cart data is held in browser memory and resets when the page is reloaded.
- The cart does not support removing items or changing quantities directly.
- Checkout is a demonstration only; no order is submitted.
- There is no backend, database, authentication, inventory system, or payment integration.
- The navigation includes demonstration sections/anchors and is not connected to a production ordering system.

## Potential Future Improvements

- Split the HTML, CSS, and JavaScript into separate files for easier maintenance.
- Add quantity controls and a remove-from-cart action.
- Persist the demo cart with local storage.
- Add a dedicated mobile navigation menu.
- Improve keyboard interaction and accessibility testing.
- Add automated tests for filtering and cart calculations.
- Replace illustrative data with a clearly labeled, original sample menu and properly licensed imagery.
- If expanding beyond a front-end demo, build a backend API and database for product data and order management.

## What I Practiced

This project provides practice with:

- Building a responsive layout using CSS Grid, Flexbox, and media queries.
- Rendering UI elements from structured JavaScript data.
- Handling user interaction with event listeners and event delegation.
- Combining category filters with text search.
- Managing cart state and calculating totals.
- Providing basic user feedback and handling image-loading failures.
- Documenting a project and communicating its scope and limitations.

## Author

**Joshua Millonado**

This project was created as a front-end web development practice project for learning and portfolio demonstration.
