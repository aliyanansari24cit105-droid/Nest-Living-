# Nest Living - Verified Student Hostel Finder

## 📖 Project Description
Nest Living is a hyper-local, web-based platform designed to connect students and parents with verified hostel and PG (Paying Guest) owners near GCT Bhakkar. It eliminates the need for unsafe physical visits and unverified Facebook listings by providing a centralized, admin-verified digital booking portal.

## ❗ Problem Statement
Students migrating for education face severe challenges in finding safe, affordable accommodation. Currently, they rely on word-of-mouth or unverified social media groups. Parents have zero visibility into hostel safety, warden details, or curfew rules. On the other hand, hostel owners lack digital presence, managing everything via paper registers, leading to overbooking and lost business.

## 🎯 Objectives
*   To provide a centralized platform for students to search, filter, and compare hostels.
*   To implement a strict Admin Verification workflow (Owner ID + Document + Physical check) to ensure 100% safe listings.
*   To offer a dedicated "Parent View" for checking safety rules and warden contacts.
*   To digitize hostel operations for owners (room availability, booking requests).

## ✨ Key Features
*   **For Students:** Advanced search, hostel comparison, roommate compatibility matching, and direct booking requests.
*   **For Parents:** A dedicated safety view to check warden details, curfew rules, and verified status before sending their child.
*   **For Owners:** Dashboard to manage room availability, accept/reject bookings, and track occupancy.
*   **For Admin:** Listing verification, dispute management, and platform analytics.

## 💻 Technology Stack
*   **Frontend:** React.js, Tailwind CSS, Axios
*   **Backend:** Node.js, Express.js
*   **Database:** MongoDB, Mongoose
*   **Authentication:** JWT (JSON Web Tokens) & bcrypt
*   **Tools:** VS Code, Git, GitHub, Postman

## 🚀 Basic Setup Instructions
*(Note: This project is currently in the development phase)*
1. Clone the repository: `git clone https://github.com/yourusername/nest-living.git`
2. Install backend dependencies: `cd server && npm install`
3. Install frontend dependencies: `cd client && npm install`
4. Create a `.env` file in the server folder and add your `MONGO_URI` and `JWT_SECRET`.
5. Run the backend: `npm run server`
6. Run the frontend: `npm start`

## 📄 Documentation
For a detailed breakdown of the development phases, architecture, and workflow, please refer to the [Implementation Plan](docs/implementation-plan.md).