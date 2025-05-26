# Shopify PDP – Test Task: BlickSolutions

This repository contains a custom Product Detail Page (PDP) implementation for a Shopify development store as part of a technical assessment for **BlickSolutions**.

This project is based on Shopify's Dawn theme.  
All custom code for the PDP is written by Stephan Pagel.


## ✅ Goal

Build a custom, fully functional, and responsive PDP that matches the provided desktop and mobile design mockups exactly in terms of:

- Typography
- Color usage
- Layout
- Gallery functionality
- Dynamic product data

## 🧰 Stack

- **Shopify CLI**
- **Shopify Dawn Theme (base)**
- **Liquid, HTML, CSS (custom section)**
- **Splide.js** (lightweight, accessible slider)

## 📦 Features

- Custom product template: `product.pdp-blicksolutions`
- Custom section: `main-product-blicksolutions.liquid`
- Fully functional image gallery (Splide.js)
  - Vertical thumbnail navigation (desktop)
  - Horizontal layout (mobile)
  - Custom navigation arrows
- Dynamic Add-to-Cart button (fully functional)
- Compare-at price, stock availability, and tax notice
- Three dynamic USP icons (editable via Theme Settings)
- Locally hosted fonts (`Montserrat` Medium + SemiBold)
- Responsive layout based on mockup hierarchy

## 🚀 How to run

1. Clone the repository and connect it to your Shopify dev store:
   ```bash
   shopify theme dev --store your-store.myshopify.com
   ```

2. Push theme to your dev store:
   ```bash
   shopify theme push
   ```

3. In the Shopify admin, assign the template `product.pdp-blicksolutions` to the product named `Neoric Neon`.

## 📁 Structure

```plaintext
templates/
└── product.pdp-blicksolutions.json

sections/
└── main-product-blicksolutions.liquid

assets/
├── splide.min.js
├── splide.min.css
├── font-montserrat-v29-latin-500.woff2
└── font-montserrat-v29-latin-600.woff2
```

## 📝 Notes

- Gallery arrows are custom elements outside the Splide container
- Arrow buttons disable automatically at start/end
- Typography overrides Shopify base styles (`base.css`) using scoped styling
- All icons and fonts are embedded locally (no external requests)

## 🔍 Preview

To preview the current dev theme:<br>
[View Theme](https://dev-test-task-blicksolutions.myshopify.com)<br>
[Customize Theme](https://dev-test-task-blicksolutions.myshopify.com/admin/themes/182252405079/editor)<br>
---

Built with ❤️ by [Stephan Pagel](https://github.com/StephanPagel)
