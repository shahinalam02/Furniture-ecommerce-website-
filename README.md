# 🛋️ Furniture E-commerce Website

## 📌 Overview

This is a **fully responsive** furniture e-commerce website built using **only HTML and CSS**. The website allows users to browse various furniture collections, view product details, and proceed to checkout. It includes multiple pages like a homepage, product pages, and a contact page.

## 📁 Project Structure

furniture-ecommerce/
│ ├── css/
│ │ ├── components/ # Shared UI components
│ │ │ └── ui.css # Styles for buttons, headers, etc.
│ │ ├── pages/ # Page-specific styles
│ │ │ ├── shop.css # Shop page styles
│ │ │ ├── cart.css # Cart page styles
│ │ │ ├── checkout.css # Checkout page styles
│ │ │ ├── product.css # Product page styles
│ │ │ ├── blog.css # Blog page styles
│ │ │ └── contact.css # Contact page styles
│ │ └── styles.css # Global styles (shared across all pages)
│ ├── images/ # Image assets (logos, banners, product images)
├── pages/
│ ├── shop.html # Shop page
│ ├── cart.html # Cart page
│ ├── checkout.html # Checkout page
│ ├── product.html # Product details page
│ ├── blog.html # Blog page
│ └── contact.html # Contact page
├── index.html # Home page
├── README.md # Project documentation

Explanation of the Structure:
public/css/: This folder contains all your CSS files.

components/: Contains styles for common UI elements like buttons, headers, etc. (ui.css).

pages/: Contains page-specific styles (e.g., shop.css, cart.css).

styles.css: Global styles that apply to all pages.

public/images/: Holds all your image assets like logos, banners, product images.

pages/: Contains HTML files for each page of the site (e.g., shop.html, cart.html).

index.html: The homepage for your e-commerce site.

Navigate to the project folder:

{ cd furniture-ecommerce }

Open index.html in a browser to view the website.

🛠️ Technologies Used
HTML5
CSS3 (including media queries for responsiveness)

🎯 Future Enhancements
Add hover effects and transitions with CSS animations.
Improve UI design with custom fonts and icons.
Add a search bar for products.

📝 License
This project is open-source under the MIT License.

---

### **How to Avoid Code Repetition in HTML & CSS (with Components)**

Since you're working purely with HTML and CSS, you'll need to **keep your code DRY (Don't Repeat Yourself)** by organizing your **CSS into reusable components**.

#### **1. Reusable Components with CSS**

- Create a **separate CSS file for reusable components** like buttons, headers, footers, etc., in the `public/css/components/` folder.

Example for a **reusable button**:

##### **`public/css/components/ui.css`**

```css
/* Reusable button styles */
.btn {
    background-color: #ff6600;
    color: white;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
    display: inline-block;
}

.btn:hover {
    background-color: #cc5500;
}

Global Styles
You can include global styles that will apply across all pages (e.g., font sizes, background colors) in the public/css/styles.css file.

public/css/styles.css
/* Global Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f9f9f9;
}

header, footer {
    background-color: #333;
    color: white;
    padding: 10px;
    text-align: center;
}
Page-Specific Styles
For each page, you'll have a separate CSS file (e.g., shop.css, cart.css) where you define styles that are specific to that page.

public/css/pages/shop.css

/* Shop Page Styles */
.shop-banner {
    background-image: url('../images/shop-banner.jpg');
    background-size: cover;
    height: 300px;
}

.product-list {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}
```
