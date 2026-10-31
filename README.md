# Nest Living — Verified Student Hostel Finder

> A verified hostel and PG booking platform for students of GCT Bhakkar, built with the MERN stack.

**Final Year Project (FYP)** · DAE CIT · Government College of Technology (GCT) Bhakkar

---

## 📖 Project Description

Nest Living is a hyper-local, web-based platform that connects students and parents with verified hostel and PG (Paying Guest) owners near GCT Bhakkar. It removes the need for unsafe physical visits and unverified Facebook listings by offering one central, admin-verified digital booking portal.

Every hostel is reviewed by an admin before it is shown to students, parents can check safety details before sending their child, and owners manage rooms and booking requests from a simple dashboard.

## ❗ Problem Statement

Students who move away for education struggle to find safe, affordable accommodation. They rely on word-of-mouth or unverified social media groups, so there is no way to know whether a listing is genuine. Parents have no visibility into hostel safety, warden details or curfew rules. Hostel owners have no digital presence and manage bookings on paper registers, which leads to overbooking and lost business.

## 🎯 Objectives

- Provide a centralised platform where students can search, filter and compare hostels.
- Implement a strict **admin verification workflow** (owner ID, property documents and review) so that only verified hostels are listed.
- Offer a dedicated **Parent View** to check safety rules, warden contacts and verified status.
- Digitise hostel operations for owners: room availability and booking requests.
- Let students review their stay and raise complaints that are tracked until resolved.

## ✨ Key Features

| Role | Features |
|------|----------|
| **Student** | Search and filter by rent, room type, gender and amenities · hostel comparison · booking requests and status tracking · roommate compatibility matching · reviews and complaints |
| **Parent** | Public, read-only safety page: verified status, warden details, curfew and house rules |
| **Owner** | Add hostels and rooms · upload verification documents · manage availability · accept or decline bookings · occupancy dashboard |
| **Admin** | Verify owner documents and approve or reject listings · handle complaints and disputes · manage users · platform statistics |

Other highlights: role-based login (JWT), responsive design for desktop and mobile, and a complete Figma UI design for all screens.

## 💻 Technology Stack

| Layer | Technology |
|-------|------------|
| Frontend | React.js, Tailwind CSS, Axios |
| Backend | Node.js, Express.js |
| Database | MongoDB (Atlas), Mongoose |
| Authentication | JWT (JSON Web Tokens) and bcrypt |
| Design | Figma |
| Tools | VS Code, Git, GitHub, Postman |
| Deployment | Vercel (frontend), Render (backend), MongoDB Atlas (database) |

## 🗂️ Project Structure

```
nest-living/
├── README.md
├── docs/
│   └── implementation-plan.md
├── server/        # Node.js + Express API
│   ├── config/
│   ├── models/
│   ├── controllers/
│   ├── routes/
│   ├── middleware/
│   └── server.js
└── client/        # React application
    └── src/
        ├── components/
        ├── pages/
        ├── services/
        └── App.js
```

## 🚀 Basic Setup Instructions

> **Note:** This project is currently in the development phase, so some features may not be available yet.

**Prerequisites:** Node.js (v18 or later), npm, Git, and a free MongoDB Atlas account.

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/nest-living.git
   cd nest-living
   ```
2. **Install backend dependencies**
   ```bash
   cd server
   npm install
   ```
3. **Install frontend dependencies**
   ```bash
   cd ../client
   npm install
   ```
4. **Create a `.env` file in the `server` folder**
   ```env
   MONGO_URI=your_mongodb_atlas_connection_string
   JWT_SECRET=your_secret_key
   PORT=5000
   CLIENT_URL=http://localhost:3000
   ```
   Never commit this file to GitHub.
5. **Run the backend** (from the `server` folder)
   ```bash
   npm run server
   ```
6. **Run the frontend** (from the `client` folder, in a second terminal)
   ```bash
   npm start
   ```
7. Open **http://localhost:3000** in your browser.

## 🛣️ Project Status

- [x] Planning and requirement analysis
- [x] System design (ERD, DFD, architecture)
- [x] UI design (Figma)
- [x] Documentation and implementation plan
- [ ] Backend development
- [ ] Frontend development
- [ ] Testing and bug fixing
- [ ] Deployment

## 📄 Documentation

For the full breakdown of architecture, workflows, modules, development phases, and the testing and deployment plans, see the **[Implementation Plan](docs/implementation-plan.md)**.

## 👤 Author

**Aliyan Ansari** · DAE CIT (Third Year) · GCT Bhakkar
Supervisor: *Abdul Saboor*