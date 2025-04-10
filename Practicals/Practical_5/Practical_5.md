# Online shopping System Workflow Analysis Report

## Introduction
The sequence diagram illustrates the comprehensive workflow of an online shopping platform, detailing interactions between seven key components: **User**, **System**, **Database**, **Seller**, **Delivery**, **Customer**, and **Payment Gateway**. This report analyzes the complete transaction lifecycle from user registration to post-purchase activities.

---

## User Authentication Flow
The workflow begins with user authentication, consisting of two primary paths:

### New User Registration:
1. User initiates by opening the signup/login form.
2. User enters registration details.
3. System queries the database to verify email uniqueness.
   - If email is already registered, an error is displayed.
   - If email is unique, the system creates a new user account.

### Existing User Login:
1. User enters login credentials.
2. System verifies credentials against database records.
3. System displays appropriate feedback for successful or failed login attempts.

---

## Product Search and Selection Process
Once authenticated, users can browse and select products through:

### Product Listing:
1. System retrieves and displays product catalog.
2. Product details are stored and managed in the database.

### Product Search:
1. User initiates product search.
2. System queries database for matching products.
3. Results are returned to user, with appropriate messaging for unfound items.

### Product Selection:
1. User selects desired product.
2. Product is added to shopping cart.
3. User can update cart contents as needed.

---

## Order Processing
The order processing workflow includes:

### Order Creation:
1. User enters shipping and billing information.
2. Order details are captured by the system.
3. Order information is stored in the database.
4. Order is transmitted to the seller.

### Order Fulfillment:
1. Seller processes the order.
2. Order status is updated in the system.
3. Order is shipped to delivery service.
4. System updates delivery status.

---

## Payment Processing
Payment handling follows a secure flow:

### Payment Verification:
1. Payment request is sent to payment gateway.
2. Gateway verifies payment details.
3. Payment status (verified or failed) is returned to the system.
4. System updates order status accordingly.

### Payment Failure Handling:
1. System processes failed payments.
2. User is notified of payment issues.

---

## Delivery and Post-Purchase Activities
The final stages of the workflow include:

### Delivery Tracking:
1. User can query delivery status.
2. System retrieves tracking information.
3. Delivery confirmation is recorded upon product receipt.

### Return Processing:
1. User can request product returns.
2. Return requests are processed by the system.
3. Seller approves or denies return requests.
4. Approved returns trigger product return process.
5. Product is returned to seller.

### Feedback Collection:
1. User submits feedback on their experience.
2. Feedback is stored in the database for future reference.

---

## Conclusion
The sequence diagram demonstrates a robust online shooping system with comprehensive handling of the entire customer journey. The workflow efficiently manages user authentication, product discovery, order processing, payment verification, delivery tracking, and post-purchase activities including returns and feedback collection.

[Link to Miro Board](https://miro.com/welcomeonboard/Q1ZJYXJxR0IzczBwWXIzYUtiWldKQ3phK2FFdlBaQlllYjA0ekZqWXA5OXZPSUw0NUNEVFUwS3VPeDBVSnFHcFNHODdZWGd0dVVRZ2ZlY2FlSFFFL0JRZklUdERIZ1oxNzlMQ2RFSGtVelp0RHIrRFBQVHMrM1JUbDRpLzdHL2NnbHpza3F6REdEcmNpNEFOMmJXWXBBPT0hdjE=?share_link_id=13176421916)
