# Comfort Shopping

Comfort Shopping is a simple e-commerce web application that allows users to browse products, add them to a cart, and manage their shopping cart. The app features a responsive design, a sidebar cart, and persistent cart storage using the browser's localStorage.

## Features

- Responsive navigation bar with burger menu for mobile devices
- Product listing section with "Add to Cart" functionality
- Sidebar cart with item quantity management (increase, decrease, remove)
- Cart total calculation and clear cart option
- Persistent cart state using localStorage
- Overlay effect when cart or menu is open

## Technologies Used

- HTML5
- CSS3
- JavaScript (ES6)
- [Font Awesome](https://fontawesome.com/) for icons

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, etc.)
- A local web server (recommended for fetching `products.json` via `fetch()`)

### Installation

1. **Clone or Download the Repository**

   ```
   git clone https://github.com/yourusername/comfort-shopping.git
   ```

   Or download and extract the ZIP file.

2. **Navigate to the Project Directory**

   ```
   cd comfort-shopping
   ```

3. **Add Product Data**

   Ensure you have a `products.json` file in the project root with the correct structure. Example:

   ```json
   {
     "items": [
       {
         "sys": { "id": "1" },
         "fields": {
           "title": "Product 1",
           "price": 19.99,
           "image": {
             "fields": {
               "file": { "url": "images/product1.jpg" }
             }
           }
         }
       }
       // ... more products
     ]
   }
   ```

4. **Start a Local Web Server**

   For example, using Python:

   ```
   # Python 3.x
   python -m http.server 8000
   ```

   Or use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension in VS Code.

5. **Open the App in Your Browser**

   Go to [http://localhost:8000](http://localhost:8000) in your browser.

## Usage

- Browse products on the main page.
- Click "Add to Cart" to add products to your cart.
- Click the cart icon to open the sidebar cart.
- Adjust quantities or remove items as needed.
- Click "Clear Cart" to empty your cart.
- The cart state is saved in your browser and will persist on reload.

## Project Structure

```
comfort-shopping/
│
├── index.html
├── style.css
├── app.js
├── products.json
├── images/
│   └── ... (product images)
└── README.md
```

## Customization

- **Add/Remove Products:** Edit `products.json` to update the product list.
- **Change Styles:** Modify `style.css` for custom appearance.
- **Update Product Images:** Place your images in the `images/` folder and update the URLs in `products.json`.

## License

This project is for educational purposes. You may use and modify it as you wish.

---

*Created by Sergiy Kochenko, 2024.*
