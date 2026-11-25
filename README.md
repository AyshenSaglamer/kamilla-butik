# Kamilla Boutique | Fashion Retail Website

A bilingual, responsive fashion retail website developed for Kamilla
Boutique, combining front-end development, interactive product
catalogues, and business-oriented digital solutions.

## 1. Project Overview

Kamilla Boutique is a multi-page fashion retail website designed
to establish a digital presence for a boutique business.

The main objective of this project was to create an elegant,
accessible, and user-friendly platform where customers can explore
fashion collections, discover new arrivals, view promotional
sections, and access store information.

This project demonstrates the practical application of software
development skills to a real-world business requirement.

## 2. Project Objectives

- Establish a digital presence for a retail business.
- Develop a responsive and visually consistent website.
- Create an organized digital product catalogue.
- Support both Turkish and English-speaking customers.
- Improve customer access to product and store information.
- Apply front-end development concepts in a practical project.
- Implement interactive functionality using JavaScript.

## 3. Technologies and Tools

| Technology | Application |
|------------|-------------|
| HTML5 | Website structure and page development |
| CSS3 | Styling, layouts, and responsive design |
| JavaScript | Dynamic content and user interactions |
| DOM API | Dynamic product card generation |
| Local Storage | Language preference management |
| CSS Grid | Responsive product catalogue layouts |
| CSS Flexbox | Component alignment and positioning |
| Google Maps | Embedded store location |
| Google Fonts | Typography and visual identity |
| Font Awesome | User interface icons |
| Git | Version control |
| GitHub | Source code management |

## 4. Development Process

### 4.1. Business Requirements and Website Planning

The project was structured around the requirements of a fashion
retail business.

The website was divided into multiple sections to make product
discovery and navigation easier for customers.

The main sections include:

- Home
- Products
- New Arrivals
- Discounts and Offers
- Contact

Product collections were further organized into individual
fashion categories.

### 4.2. Website Structure and Navigation

A multi-page website architecture was implemented using HTML.

Separate pages were created for different product categories,
allowing customers to browse collections independently.

The navigation system connects the homepage, product categories,
promotional sections, and contact page.

The implementation includes:

- Navigation menus
- Internal page linking
- Category-based product browsing
- Return-to-home navigation
- Turkish and English navigation labels

### 4.3. User Interface and Visual Design

CSS was used to establish a consistent visual identity across
the website.

The design focuses on an elegant fashion retail experience
through typography, product photography, spacing, and layout.

The implementation includes:

- Customized typography
- Boutique-oriented visual design
- Product cards
- Hover effects
- Interactive navigation elements
- Image-based product presentation
- Consistent visual styling
- Font Awesome icons
- Google Fonts integration

### 4.4. Responsive Web Design

Responsive design techniques were implemented to support
different screen sizes.

CSS Grid and Flexbox were used to organize content and product
cards according to the available screen space.

Media queries were implemented to adjust selected layouts
for smaller screens.

The responsive design implementation includes:

- Flexible page layouts
- Adaptive product grids
- Mobile-oriented navigation adjustments
- Responsive content alignment
- Flexible product image presentation

### 4.5. Product Catalogue Development

The product catalogue was organized into multiple fashion
categories, including:

- Upper Wear
- Lower Wear
- Dresses
- Evening Dresses
- Jackets
- Matching Sets
- Jumpsuits
- Bags
- Accessories

Individual category pages were developed to display relevant
product collections.

Product images were organized within a dedicated image directory
to support structured asset management.

### 4.6. Dynamic Product Card Generation

JavaScript was used to dynamically generate product cards
on selected product category pages.

Instead of manually creating every product card in HTML,
product information was organized into JavaScript arrays.

Each product object contains information such as:

- Turkish product name
- English product name
- Product image path

The implementation uses JavaScript iteration and DOM
manipulation to generate and display product cards.

Example of the product data structure:

```javascript
const products = [
  {
    name_tr: "Bluz",
    name_en: "Blouse",
    image: "images/Bluz 1.jpeg"
  }
];
```

The application iterates through the product array and
dynamically creates HTML elements for each product.

This approach demonstrates:

- JavaScript arrays and objects
- Iteration using forEach()
- Dynamic HTML generation
- DOM manipulation
- Structured product data management
- Separation of product data and presentation

It also makes adding or modifying products easier without
manually rewriting the complete page structure.

### 4.7. Multilingual Website Development

A bilingual interface was implemented to support both Turkish
and English-speaking customers.

Language selection is managed through JavaScript functions
that update displayed website content.

The language system includes:

- Turkish and English language options
- Interactive language selection buttons
- Dynamic navigation text updates
- Product name translations
- Contact information translations
- Language-specific content visibility

HTML data attributes were used on selected pages to store
translated product names.

Example:

```html
<h3 data-tr="Bluz" data-en="Blouse">
  Bluz
</h3>
```

JavaScript retrieves the appropriate translation according
to the selected language and updates the displayed content.

### 4.8. Language Preference Management

Browser Local Storage was implemented on selected product
category pages to remember the user's language preference.

When a customer selects a language, the preference is stored
in the browser.

```javascript
localStorage.setItem("lang", lang);
```

The stored preference can then be retrieved when the
corresponding page is loaded again.

```javascript
const savedLang =
  localStorage.getItem("lang") || "tr";
```

This implementation demonstrates:

- Client-side data persistence
- Browser Storage API usage
- User preference management
- Dynamic interface customization

### 4.9. New Arrivals and Promotional Sections

Dedicated pages were created for new arrivals and discounts.

These sections were designed to help the business highlight
new collections and promotional products independently
from the main product catalogue.

This structure supports future content updates and
marketing activities.

### 4.10. Contact and Location Integration

A dedicated contact page was developed to provide customers
with access to boutique information.

The contact page includes:

- Store contact information
- Social media information
- Embedded Google Maps
- Turkish and English content

Google Maps integration allows customers to view the
store location directly from the website.

### 4.11. Asset and Source Code Management

Website resources were organized into dedicated directories.

Product photographs, logos, and language selection icons
were stored in the images directory.

Shared styling resources were organized in the styles
directory, alongside page-specific styling.

Git and GitHub were used to manage the project's source
code and maintain an accessible project repository.

## 5. Project Architecture

The website follows a client-side, multi-page architecture.

    User
      |
      v
    Web Browser
      |
      v
    HTML Pages
      |
      +-- CSS Styling
      |
      +-- JavaScript Logic
      |     |
      |     +-- Product Data Arrays
      |     +-- Dynamic Product Cards
      |     +-- Language Management
      |     +-- Local Storage
      |
      +-- Image Assets
      |
      +-- External Services
            |
            +-- Google Maps
            +-- Google Fonts
            +-- Font Awesome

The application runs directly in the user's browser
without requiring a dedicated application server.

## 6. Repository Structure

    kamilla-butik/
    |
    |-- Kamilla Butik/
    |   |-- index.html
    |   |-- urunler.html
    |   |-- ustgiyim.html
    |   |-- altgiyim.html
    |   |-- elbiseler.html
    |   |-- abiye.html
    |   |-- ceket.html
    |   |-- takimlar.html
    |   |-- tulumlar.html
    |   |-- cantalar.html
    |   |-- aksesuarlar.html
    |   |-- yenigelenler.html
    |   |-- indirimler.html
    |   |-- iletisim.html
    |   |
    |   |-- images/
    |   |
    |   |-- styles/
    |       |-- style.css
    |
    |-- README.md

## 7. Getting Started

### Prerequisites

- A modern web browser
- Git (optional)
- Visual Studio Code (optional)

### Installation

Clone the repository:

```bash
git clone https://github.com/AyshenSaglamer/kamilla-butik.git
```

Navigate to the project directory:

```bash
cd kamilla-butik
cd "Kamilla Butik"
```

Open `index.html` in a web browser.

No additional package installation is required for the
client-side website.

An internet connection is required to load external
services such as Google Maps and Google Fonts.

## 8. Skills Demonstrated

### Technical Skills

- Front-end web development
- HTML5 and CSS3
- JavaScript programming
- DOM manipulation
- Arrays and objects
- Dynamic content generation
- Responsive web design
- CSS Grid and Flexbox
- Browser Local Storage
- Multilingual interface development
- Third-party service integration
- Git and GitHub

### Software Engineering Skills

- Requirements-oriented development
- Multi-page application architecture
- Source code organization
- Structured data management
- User interface development
- Problem-solving
- Business-oriented software development

## 9. Business Value

The website provides a digital platform through which
a boutique business can present its products and
communicate with potential customers.

The project aims to support:

- Digital brand visibility
- Product discoverability
- Customer accessibility
- Multilingual customer communication
- Store location accessibility
- Promotional content presentation

## 10. Future Enhancements

Potential future improvements include:

- Database integration
- Automated product management
- Product search and filtering
- Inventory management system
- Administrative dashboard
- Customer authentication
- Shopping cart functionality
- Online payment integration
- Customer behavior analytics
- Personalized product recommendations
- AI-powered fashion recommendation system

These enhancements could transform the current digital
catalogue into a more comprehensive e-commerce platform.

## 11. Project Status

Completed — Front-end fashion retail website.

The current version focuses on product presentation,
multilingual functionality, and digital business visibility.

Full e-commerce transactions and backend functionality
are outside the scope of the current implementation.

## 12. Developer

**Ayshen Saglamer**

Computer Engineering & Economics and Finance Student

Areas of Interest:

- Software Engineering
- Artificial Intelligence
- Data Science
- Financial Technology
- Business-Oriented Software Development

GitHub: https://github.com/AyshenSaglamer

## 13. Copyright

All rights reserved © 2025 Ayshen Saglamer.

This project may not be copied, modified, or redistributed
without prior permission.
