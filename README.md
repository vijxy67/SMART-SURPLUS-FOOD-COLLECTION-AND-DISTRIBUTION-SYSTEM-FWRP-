# Smart Food Waste Reduction and Redistribution Platform (FWRP)

## Project Overview

The Smart Food Waste Reduction and Redistribution Platform (FWRP) is a web-based application designed to facilitate the donation and distribution of surplus food. It aims to connect food donors with individuals and organizations in need, helping reduce avoidable food waste and encouraging responsible food sharing.

The application provides an interface for user registration and login, food donation management, available-food listings, pickup location visualization, food-claim confirmation, and basic administrator monitoring.

The current implementation is a front-end prototype built using HTML, CSS, and JavaScript, with browser Local Storage used to store user and donation records.

## Problem Statement

Food waste and food insecurity are major social challenges. While households, restaurants, and event organizers may have surplus food, many people and charitable organizations struggle to access sufficient food. The absence of an organized and accessible coordination platform can make it difficult to identify available donations, communicate pickup details, and collect food before its expiry.

FWRP addresses this problem by providing a centralized web interface for recording surplus food donations and displaying available food items with their quantities, expiry dates, donor contact information, and pickup addresses.

The system aims to improve coordination between donors and recipients, promote food redistribution, reduce avoidable food waste, and support a more sustainable and socially responsible food-sharing process.

## Objectives

- Reduce avoidable food waste through food donation and redistribution.
- Provide a simple interface for registering users and accessing the platform.
- Allow donors to submit food item details and pickup information.
- Display available donations for potential recipients.
- Provide map views to help users identify collection locations.
- Support basic food-claim confirmation.
- Provide an administrator dashboard for viewing registered users and donation counts.
- Promote community participation and sustainable food management.

## Technologies Used

### Programming Languages

- **HTML5:** Defines the structure of the web pages, forms, buttons, dashboard sections, and content.
- **CSS3:** Provides visual styling, page layouts, colors, glassmorphism effects, responsive grid layouts, hover effects, and animations.
- **JavaScript (ES6+):** Implements application logic, navigation, registration and login validation, donation handling, dynamic content rendering, notifications, and Local Storage operations.

### Libraries and External Resources

- **Font Awesome 6.0.0:** Provides icons for navigation, authentication, food donations, locations, and notifications.
- **Google Maps Embed:** Displays map views for donation and pickup addresses.
- **Unsplash:** Supplies the background image.
- **Google logo SVG:** Displays the Google logo on the authentication interface.
- **Browser Local Storage API:** Stores user and donation records locally in the browser.
- **JavaScript DOM API:** Enables dynamic updates to HTML elements and interface sections.

### Development Approach

The project uses vanilla HTML, CSS, and JavaScript. It does not currently use a front-end framework, external JavaScript package manager, server-side application, or dedicated database.

## Main Features

### 1. User Authentication Interface
- User registration and login forms.
- Email-based account lookup.
- Basic password validation.
- Duplicate email checking during registration.
- Success and error notifications.

### 2. Food Donation Management
- Donor name and phone number fields.
- Food item and quantity information.
- Expiry date and time entry.
- Pickup address entry.
- Map visualization for the entered address.
- Local storage of donation records.

### 3. Food Availability and Collection
- Display of recorded food donations.
- Food item, quantity, expiry time, and address information.
- Selection of a donation to inspect its details.
- Pickup map visualization.
- Food-claim confirmation messages.

### 4. Administrator Dashboard
- Administrative login interface.
- Total registered user count.
- Total recorded donation count.
- Display of registered user details.
- Basic monitoring of application records.

### 5. User Interface and Notifications
- Glassmorphism-inspired card design.
- Background image with a dark overlay.
- Font Awesome icons.
- Hover effects and CSS animations.
- Animated success and error notifications.
- Navigation between application sections.

## Implementation Details

### HTML
HTML defines the page structure and includes the login interface, administrator portal, dashboards, donation forms, donation listings, maps, and confirmation screen.

### CSS
CSS is embedded in the `<style>` element in `main.html`. It uses Flexbox, CSS Grid, pseudo-classes, pseudo-elements, transitions, keyframe animations, and backdrop filters to create the user interface.

### JavaScript
JavaScript is embedded in the `<script>` element. It manages page navigation, registration, login checks, donation creation, donation listing, administrator statistics, map updates, and notifications.

### Data Storage
The application uses the browser's Local Storage API with two primary keys:

- `fwrp_users` — stores registered user records.
- `fwrp_donations` — stores food donation records.

Data is serialized with `JSON.stringify()` and retrieved with `JSON.parse()`. Records are stored in the browser rather than in a centralized server database.

## Application Workflow

1. Open the application in a web browser.
2. Register a new account or log in using an existing account.
3. Access the main dashboard.
4. Choose to donate food or browse available donations.
5. Enter donation details or select a recorded food item.
6. View the pickup address and associated map.
7. Receive a confirmation notification.
8. Use the administrator interface to inspect registered users and donation statistics.

## Current Limitations

- User and donation data are stored locally in the browser.
- Data is not shared across different users or devices through a central database.
- Authentication is a basic client-side demonstration and is not suitable for production use.
- The Google sign-in button is a placeholder and does not perform actual OAuth authentication.
- The administrator password is hardcoded in the JavaScript.
- Donation claiming currently displays a confirmation message; it does not implement a complete reservation, collection, or status-tracking workflow.
- Map integration uses embedded map URLs rather than a full location-management backend.
- Food safety verification, donor verification, and automated expiry monitoring are not implemented as complete workflows.

## Future Enhancements

- Integrate a backend using Node.js and Express or another suitable server-side framework.
- Use a database such as MySQL, PostgreSQL, or MongoDB.
- Implement secure authentication and role-based access control.
- Integrate Google OAuth for actual Google sign-in.
- Add food availability filters and expiry-based sorting.
- Implement donation reservation, collection status, and cancellation workflows.
- Add automated notifications for expiring food and confirmed collections.
- Improve location selection and distance-based donation discovery.
- Add donation analytics and reporting.
- Deploy the application for access across multiple users and devices.

## Expected Impact

FWRP aims to make surplus food easier to discover and redistribute by improving communication between food donors and recipients. With further development, the platform could support community food banks, NGOs, restaurants, households, and volunteers in coordinating food donations more effectively.

## Conclusion

The Smart Food Waste Reduction and Redistribution Platform demonstrates how web technologies can be used to address food waste and food accessibility challenges. Its current prototype provides a foundation for food donation entry, donation browsing, location visualization, user interfaces, and basic administration. Future integration with secure authentication, a centralized database, and a backend service can help transform it into a more reliable, scalable, and practical food redistribution system.

## License

Choose an appropriate open-source license before publishing the project, such as the MIT License, if you want others to reuse and modify the code.
