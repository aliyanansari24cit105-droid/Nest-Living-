# Nest Living - Implementation Plan

## 1. Project Overview & Objectives
**Project Name:** Nest Living
**Objective:** To build a verified student hostel finder specifically for the GCT Bhakkar area. The system aims to solve the trust deficit in hostel hunting by introducing an admin-verification layer and a dedicated parent safety portal, while providing owners with a digital management dashboard.

## 2. Proposed Technology Stack
*   **MongoDB:** NoSQL database for flexible, JSON-like storage of hostel details and user data.
*   **Express.js:** Backend framework for handling API routing and business logic.
*   **React.js:** Frontend library for building a fast, dynamic Single Page Application (SPA).
*   **Node.js:** JavaScript runtime environment for the server.
*   **Tailwind CSS:** For rapid, mobile-responsive UI development.
*   **JWT:** For secure, role-based authentication (Admin, Owner, Student).

## 3. Project Architecture & Workflow
The application follows a standard **Client-Server Architecture**:
1.  **Client (React):** The UI where users interact. Sends HTTP requests via Axios.
2.  **Server (Express/Node):** Receives requests, validates data, and processes logic.
3.  **Database (MongoDB):** Stores and retrieves data. The server uses Mongoose to communicate with MongoDB.

**Data Flow Example:** 
A student clicks "Search Hostels" -> React sends a `GET` request to the Express API -> Express queries MongoDB -> MongoDB returns the data -> Express sends a JSON response to React -> React renders the hostel cards.

## 4. Main Features & Modules
*   **Auth Module:** Registration, login, and role-based access control.
*   **Student Module:** Search hostels, filter by price/gender, view details, send booking request, roommate matching.
*   **Owner Module:** Upload documents for verification, manage room availability, view booking dashboard.
*   **Admin Module:** Verify owner documents, approve/reject listings, manage reported disputes.
*   **Parent Module:** Read-only access to safety rules, warden details, and verified status.

## 5. Development Phases & Implementation Steps (16-Week Timeline)

*   **Phase 1: Planning & Design (Weeks 1-2)**
    *   Finalize requirements and create ERD (Database Schema).
    *   Design UI wireframes for all dashboards.
*   **Phase 2: Backend Development (Weeks 3-6)**
    *   Set up Express server and connect MongoDB.
    *   Develop REST APIs for Auth, Hostels, Rooms, and Bookings.
    *   Test all APIs using Postman.
*   **Phase 3: Frontend Development (Weeks 7-12)**
    *   Set up React and configure routing.
    *   Build UI components (Search, Cards, Forms).
    *   Integrate frontend with backend APIs using Axios.
*   **Phase 4: Testing & Bug Fixing (Weeks 13-14)**
    *   Conduct end-to-end testing (e.g., Can a student actually book a room?).
    *   Fix UI responsiveness issues and logic bugs.
*   **Phase 5: Deployment & Documentation (Weeks 15-16)**
    *   Deploy Frontend to Vercel and Backend to Render.
    *   Host Database on MongoDB Atlas (Free Tier).
    *   Write final project report.

## 6. Testing & Deployment Plans
*   **API Testing:** All backend routes will be tested using Postman to ensure correct status codes and data formats.
*   **Manual Testing:** Testing the complete user journey from both Student and Owner perspectives.
*   **Deployment:** 
    *   **Frontend:** Vercel (Free tier, automatic deployment from GitHub).
    *   **Backend:** Render (Free tier for Node.js apps).
    *   **Database:** MongoDB Atlas (Cloud database).