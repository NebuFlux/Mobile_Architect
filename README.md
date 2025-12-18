# MyInventory App

![App Logo](path/to/logo.png) 

A mobile inventory management application built for Android, designed to streamline warehouse operations by providing efficient inventory tracking, user authentication, and real-time notifications. This app addresses the needs of warehouse laborers, supervisors, and executives by enabling secure access to inventory data, quick updates, and alerts for low stock levels.

## Table of Contents

- [Description](#description)
- [Features](#features)
- [Screenshots](#screenshots)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Development Process](#development-process)
- [Testing](#testing)
- [Challenges and Innovations](#challenges-and-innovations)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Description

The MyInventory app is developed to meet the requirements of a robust inventory management system. Its primary goals include:
- Maintaining accurate and centralized inventory records using a relational database.
- Providing role-based user accounts for secure access and appropriate permissions.
- Sending automated notifications when item quantities reach zero to prevent stockouts.
- Offering a user-centered interface for efficient inventory queries, updates, and additions.

This app addresses user needs such as real-time inventory visibility for laborers, trend analysis for supervisors, and high-level data insights for executives, ensuring seamless warehouse management.

## Features

- **User Authentication**: Secure login and sign-up screens with password hashing using BCrypt for enhanced security.
- **Inventory Grid View**: A searchable grid displaying items in rows of three, with options to add items, filter/search, and delete entire rows.
- **Item Details View**: Detailed screen for viewing and editing item information, including name, price, quantity, description, location (shelf/aisle), and image.
- **Add Item Functionality**: Form-based screen for adding new items with image capture via camera and location selection via dropdowns.
- **Low Stock Notifications**: SMS alerts sent to users when an item's quantity reaches zero, with permission handling for camera and SMS.
- **Role-Based Access**: Supports different user roles (e.g., Laborer, Supervisor) to control features and data access.
- **Search and Filtering**: Real-time search for items by name, with visual indicators for active filters.
- **Data Persistence**: Uses Room database for storing items and users, ensuring data integrity and offline access.

## Screenshots

<!-- Add actual screenshots here -->
- **Login Screen**: Hero image with username/password fields and sign-up link.  
  ![Login Screen](path/to/login-screenshot.png)
- **Grid View Screen**: Inventory grid with add and filter buttons.  
  ![Grid View](path/to/grid-screenshot.png)
- **Item View Screen**: Editable item details with increment/decrement controls.  
  ![Item View](path/to/item-screenshot.png)
- **Add Item Screen**: Input fields with camera integration and location dropdowns.  
  ![Add Item](path/to/add-item-screenshot.png)
- **Sign Up Screen**: Form for creating accounts with validation.  
  ![Sign Up](path/to/signup-screenshot.png)

## Installation

To set up the project locally:

1. Clone the repository:
