---
description: Repository Information Overview
alwaysApply: true
---

# Comercial-React Shop Information

## Summary
A lightweight, static web-based shop application and management system. The project provides a customer-facing "Mini Commercial Shop" interface and a "Dashboard" for administrative tasks such as adding products and managing dynamic pages. It utilizes **React 18** and **Babel** via CDN for a modern frontend experience without requiring a Node.js build environment.

## Structure
- [./Comercials_Show/](./Comercials_Show/): Contains the main customer-facing shop application.
- [./Dashboard/addeditems/](./Dashboard/addeditems/): Contains administrative tools for product and page management.
- [./images/](./images/): Repository for product images and assets.
- [./.zencoder/](./.zencoder/): Configuration for Zencoder workflows.

## Language & Runtime
**Language**: HTML5, JavaScript (ES6+), CSS3  
**Framework**: React 18 (via CDN)  
**Version**: N/A (Client-side execution)  
**Build System**: None (Static files)  
**Package Manager**: None (Dependencies loaded via CDN)

## Dependencies
**Main Dependencies**:
- **React**: Frontend library (version 18, via unpkg)
- **ReactDOM**: Browser-specific methods for React (version 18, via unpkg)
- **Babel Standalone**: In-browser JSX/ES6 translation (via unpkg)
- **SweetAlert2**: Beautiful popup notifications (via cdnjs/jsdelivr)

## Build & Installation
This project is a static site and does not require installation or a build process.
```bash
# No installation required. Open HTML files directly in a browser.
```

## Key Resources
**Main Files**:
- [./Comercials_Show/Comercial.html](./Comercials_Show/Comercial.html): Main entry point for the shop interface.
- [./Dashboard/addeditems/page_manager.html](./Dashboard/addeditems/page_manager.html): Main entry point for managing shop pages.
- [./Dashboard/addeditems/additem.html](./Dashboard/addeditems/additem.html): Interface for adding new products to the shop.
- [./Comercials_Show/Comercial.json](./Comercials_Show/Comercial.json): Initial product data storage.

**Configuration Structure**:
- **Data Persistence**: Uses `localStorage` to persist custom products and page configurations (`shopItems_*`, `shopPages`, `customProducts`).
- **Asset Management**: Images are stored in the [./images/](./images/) directory and referenced by filename in product data.

## Usage & Operations
**Key Operations**:
- **Adding Products**: Use the `additem.html` dashboard to add new items, which are saved to `localStorage`.
- **Managing Pages**: Use `page_manager.html` to create or modify shop categories/pages.
- **Shopping**: Users can browse items in `Comercial.html`, add them to a cart, and "checkout" (simulated).

## Validation
**Quality Checks**:
- Manual verification of React component rendering and `localStorage` updates.
- Basic error handling for `fetch` operations on JSON data and `JSON.parse` for local storage.
