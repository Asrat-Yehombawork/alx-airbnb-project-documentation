# Use Case Documentation for Airbnb Clone Backend

This document outlines the use cases for the backend of the Airbnb Clone project. It describes the system's functionality from the perspective of different user roles, including **Guests**, **Hosts**, **Admins**, and the **System** itself. These use cases serve as a guide for designing and implementing the backend system.

---

## 🎯 Purpose

The purpose of this document is to capture the requirements and interactions between users and the system, ensuring the backend architecture meets the functional and technical needs of the Airbnb Clone platform.

---

## 📝 Use Case Overview

### **Actors**
- **Guest**: A user looking to book properties.
- **Host**: A user who lists properties for guests.
- **Admin**: A user responsible for managing the platform's content and user activities.
- **System**: The backend system that handles authentication, bookings, notifications, and payments.

### **Use Cases**
The table below outlines the primary use cases categorized by actor:

| **Actor**       | **Use Case**                                                                                                                                                   | **Description**                                                                                                                                                     |
|------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Guest**        | **Register**                                                                                                                                                 | A guest registers for an account using email or OAuth authentication.                                                                                               |
|                  | **Login**                                                                                                                                                    | A guest logs into their account securely.                                                                                                                           |
|                  | **Update Profile**                                                                                                                                           | A guest updates their profile information and uploads a profile photo.                                                                                              |
|                  | **Search Properties**                                                                                                                                        | A guest searches for properties by location, price, amenities, and availability.                                                                                    |
|                  | **Book a Property**                                                                                                                                          | A guest selects a property and books it for specific dates.                                                                                                         |
|                  | **Pay for Booking**                                                                                                                                          | A guest completes a secure payment for their booking.                                                                                                               |
|                  | **Cancel Booking**                                                                                                                                           | A guest cancels a booking as per the cancellation policy.                                                                                                           |
|                  | **Leave Reviews**                                                                                                                                             | A guest leaves a review and rating for a property after their stay.                                                                                                 |
| **Host**         | **Register**                                                                                                                                                 | A host registers for an account using email or OAuth authentication.                                                                                                |
|                  | **Login**                                                                                                                                                    | A host logs into their account securely.                                                                                                                            |
|                  | **Create Property Listing**                                                                                                                                  | A host adds a property listing with details such as title, description, price, and availability.                                                                    |
|                  | **Edit/Delete Listing**                                                                                                                                      | A host edits or removes their property listings.                                                                                                                    |
|                  | **View Bookings**                                                                                                                                            | A host views bookings for their properties to see reserved dates.                                                                                                   |
|                  | **Cancel Booking**                                                                                                                                           | A host cancels a booking due to unforeseen circumstances.                                                                                                           |
|                  | **Respond to Reviews**                                                                                                                                       | A host responds to reviews to provide additional context or address feedback.                                                                                       |
|                  | **Receive Notifications**                                                                                                                                    | A host receives notifications for new bookings, cancellations, or payments.                                                                                        |
| **Admin**        | **Manage Users**                                                                                                                                             | An admin views and manages all user accounts, ensuring platform integrity.                                                                                          |
|                  | **Manage Properties**                                                                                                                                        | An admin monitors and manages property listings, removing inappropriate or fraudulent content.                                                                      |
|                  | **Monitor Bookings**                                                                                                                                         | An admin monitors booking statuses and resolves conflicts between users if necessary.                                                                               |
|                  | **Oversee Payments**                                                                                                                                         | An admin tracks payment transactions and resolves issues such as payment failures.                                                                                  |
| **System**       | **Authenticate Users**                                                                                                                                       | The system validates user credentials and issues JWTs for secure sessions.                                                                                          |
|                  | **Handle Payments**                                                                                                                                          | The system integrates with payment gateways to process transactions securely.                                                                                       |
|                  | **Send Notifications**                                                                                                                                       | The system sends email and in-app notifications to users for booking confirmations, cancellations, and payment updates.                                             |
|                  | **Prevent Double Bookings**                                                                                                                                  | The system ensures that a property cannot be booked for overlapping dates.                                                                                          |
|                  | **Store Data**                                                                                                                                               | The system stores property details, user data, booking information, and reviews in a relational database.                                                           |

---

## 🔄 System Flow

The following is the interaction flow between actors and the system:
1. **Guests and Hosts** register, log in, and interact with the platform through the backend API.
2. **Admins** monitor and manage user and system activities using the admin dashboard.
3. The **System** ensures smooth operations by validating user actions, storing data, and integrating with third-party services (e.g., payment gateways).

---

## 📚 Usage

This use case documentation can be used for:
- **Developers**: To understand system requirements and design backend features.
- **Project Managers**: To prioritize functionality based on use cases.
- **Testers**: To create test cases ensuring all use cases are implemented correctly.

---

## 🛠️ Contributions

Contributions to extend or refine these use cases are welcome! Feel free to submit a pull request or open an issue for discussions.
