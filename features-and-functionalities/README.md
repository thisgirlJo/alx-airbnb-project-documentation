## 🟦 Central Node:

### **Airbnb Clone Backend System**

↙️ ↘️ Connects to the main functional modules below.

1. User Management

- Register / Login (JWT)
- Password Hashing (bcrypt)
- Role-based Access (guest, host, admin)
- Update Profile

**Connects to:**

- Database (Users Table)
- Security Module (for Auth & Roles)

2. Property Management

- Add / Edit / Delete Property
- View Properties
- Search / Filter Listings

**Connects to:**

- User Management (Host creates listings)

- Booking System (Properties can be booked)

- Database (Properties Table)

3. Booking System

- Create / Update / Cancel Bookings
- Booking History
- Status (pending, confirmed, canceled)

**Connects to:**

- User Management (Guests & Hosts)
- Property Management (Linked to properties)
- Payment Processing (For confirmed bookings)
- Database (Bookings Table)

4. Payment Processing

- Integrate Stripe / PayPal
- Handle Refunds
- Record Transactions

**Connects to:**

- Booking System (Triggered after confirmation)
- Database (Payments Table)
- Security Module (For safe transactions)

5. Reviews & Ratings

- Submit Review
- Rate Property (1–5 stars)
- Display Average Rating

**Connects to:**

- User Management (Review author)
- Property Management (Reviewed property)
- Database (Reviews Table)

6. Messaging System

- Send Message (guest ↔ host)
- View Conversation History

**Connects to:**

- User Management (sender & recipient)
- Database (Messages Table)

7. Admin Panel

- Manage Users / Properties / Bookings
- Monitor Payments
- Handle Reports

**Connects to:**

- All modules (User, Property, Booking, Payments)
- Database (for full control access)

8. Security Module

- Authentication (JWT)
- Authorization (Role-based)
- Input Validation
- Rate Limiting

**Connects to:**

- All modules (protects every API route)
- Database (secure data storage)

### 🔗 Supporting Components

9. Database

- Tables: Users, Properties, Bookings, Payments, Reviews, Messages

10. External APIs

- Stripe / PayPal (Payments)
- Cloud Storage (Images)
- Geolocation (Property location)