Version 1.4 - Order Confirmation & Receipt System
Added
- Transaction ID Generator: Implemented a feature to generate a unique random Transaction ID (e.g., PK-82931) upon checkout, serving as the customer's receipt number.
- Customer Nickname Field: Added a required input field for customers to enter their nickname, facilitating easier identification for delivery drivers or pickup staff.
- Order Success Screen: Created a new UI container that displays the final receipt details (Customer Name, File, Price, Transaction ID) after a successful order.

Changed
- Form Submission Flow: Refactored the checkout process to hide the order form and display the success screen upon submission, preventing duplicate orders and providing clear feedback to the user.
- UI Structure: The main upload section now conditionally displays either the Form or the Receipt view.

Version 1.3 - Dynamic Address Input
Added
- Conditional Address Field: A "Delivery Address" input field now dynamically appears only when the user selects "Deliver to my Address" from the dropdown.
- Input Validation: Added form validation to ensure the address field is not empty if delivery is selected before submission.
Changed
- Event Handling: Refactored the delivery dropdown logic to handle both price updates and UI visibility simultaneously.

UI/UX:
- Applied a distinct yellow background style to the address field to draw attention when it appears.
- Added a smooth fade-in animation for the address field toggle.

Version 1.2 - Dynamic Pricing Update
Added
- Live Price Calculator: Implemented a dynamic pricing engine that calculates the total cost instantly as the user selects options.
- Price Breakdown UI: Added a visual summary section showing the math behind the total (e.g., "5 x ₱5.00 + ₱40.00 Delivery").
- Data Attributes: Integrated data-price and data-fee attributes into HTML select options to store pricing logic on the frontend.
- Form Validation: Added a basic submit event listener to handle order processing simulation.

Changed
- Input Styling: Updated CSS to support the new price summary container and improved input field consistency.

Version 1.0
Features
- Core UI Structure: Established the main layout with a sticky header, hero section, order form, and footer.
- Responsive Design: Implemented a mobile-first design using CSS Grid and Flexbox that adapts to different screen sizes.
- File Upload Interface: Created a drag-and-drop zone (click-to-browse) supporting multiple file formats (PDF, DOCX, JPG, PNG, CDR).
- Order Configuration Form:
- Paper/Material selection (A4, Legal, Sticker, Photo, Tarpaulin).
- Quantity input field.
- Delivery options (Pick-up vs. Delivery).
- Color mode selection (Black & White vs. Colored).
- Special instructions text field.
- Services Showcase: Added an informational section displaying available printing categories (Documents, Marketing, Stickers, Tarpaulins).
- Basic File Handling: JavaScript functionality to display the selected filename upon upload.
- Branding: Applied the "PrintKita" brand colors (Blue/Green) and logo.
