# MyInventory App

![App Logo](/login_image) 

A mobile inventory management application built for Android, designed to streamline warehouse operations by providing efficient inventory tracking, user authentication, and real-time notifications. This app addresses the needs of warehouse laborers, supervisors, and executives by enabling secure access to inventory data, quick updates, and alerts for low stock levels.

## Table of Contents

- [Description](#description)
- [Features](#features)
- [Screenshots](#screenshots)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Development Process](#development-highlights)
- [Testing](#testing)
- [Challenges and Innovations](#challenges-and-innovations)
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

- **Login Screen**: Hero image with username/password fields and sign-up link.  
  ![Login Screen](/Login.png)
- **Grid View Screen**: Inventory grid with add and filter buttons.  
  ![Grid View](/GridView.png)
- **Item View Screen**: Editable item details with increment/decrement controls.  
  ![Item View](/ItemDetails.png)
- **Add Item Screen**: Input fields with camera integration and location dropdowns.  
  ![Add Item](/AddItem.png)
- **Sign Up Screen**: Form for creating accounts with validation.  
  ![Sign Up](/SignUp.png)

## Installation

To set up the project locally:

1. Download the [My_Inventory Project ZIP](/My_Inventory.zip) and extract it, or clone the repository:
2. Open in Android Studio (Arctic Fox or later).
3. Sync Gradle and build the project.
4. Run on an emulator or physical device (API 24+ recommended).

## Usage

1. Launch the app and log in with existing credentials or sign up for a new account.
2. Navigate to the Grid View to browse/search inventory.
3. Click an item to view/edit details, or use the add button to create new items.
4. Receive SMS notifications for low stock (ensure SMS permission is granted).
5. Use the back navigation or delete options as needed.

The application uses Contextual Permissions

## Technologies Used

- **Kotlin** → Primary language
- **Jetpack Compose** → Declarative UI
- **Room Persistence Library** → Local database
- **MVVM Architecture** → With ViewModels, LiveData, and Coroutines
- **Coil** → Async image loading
- **Accompanist Permissions** → Runtime permission handling
- **BCrypt** → Secure password hashing
- **Kotlin Serialization** → Type-safe navigation

## Development Highlights

The app follows clean MVVM patterns with type-safe navigation and efficient state management. Particular success was achieved in UI layout and theming, using custom Material 3 color schemes for a consistent, modern look.

Strategies included:
- Type-safe navigation with Kotlin Serialization for routes.
- Derived states and remember keys for efficient recomposition in Compose.
- Asynchronous database operations to prevent UI blocking.

These techniques promote maintainable code and can be applied in future projects for scalable Android apps.

Innovations include:
- Custom row deletion in the grid view (chunked items + batch delete).
- Robust SMS alert system with phone number dialog and session-based deduplication.

## Testing

Testing was conducted through iterative trial-and-error on emulators and physical devices:
- Verified UI interactions (e.g., form validations, navigation flows).
- Tested database operations (insert, update, delete) with edge cases like empty queries.
- Simulated SMS sending and camera capture to ensure permissions and functionality.
- Checked for crashes, memory leaks, and UI responsiveness across screen sizes.

## Challenges and Innovations

- **Grid Screen Deletion**: Innovated a row-based deletion mechanism in the grid view, allowing bulk deletion of items in groups of three. This required custom chunking of items and handling batch deletes in the repository.
- **SMS Phone Number Handling**: Overcame challenges in securely obtaining and storing user phone numbers by implementing a dialog for input, integrated with permission wrappers and database updates. This ensured accurate notifications without compromising privacy.

The layout and theming were particularly successful, adhering to Material Design 3 principles with custom color schemes and responsive modifiers, demonstrating strong skills in creating intuitive, visually consistent UIs.

Joshua Shoemaker  
GitHub: [NebuFlux](https://github.com/NebuFlux)
