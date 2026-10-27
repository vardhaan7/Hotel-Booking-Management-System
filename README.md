

# The Wild Oasis – Booking Dashboard

A **full-stack booking management dashboard** built with **React (Vite) + Styled Components** for the frontend and **Supabase (PostgreSQL + Auth + Storage)** for the backend.

This project allows hotel staff and admins to manage cabins, bookings, guests, and user roles in one place, with real-time analytics and secure authentication.

---

## 🚀 Project Description

The **Wild Oasis** dashboard is designed to simplify hotel and resort operations. It provides:

* A **Dashboard** with KPIs (bookings, occupancy, revenue).
* **CRUD for Cabins** – add, edit, delete rooms with images and discounts.
* **CRUD for Bookings** – manage reservations, check-in/out guests, handle cancellations.
* **Guest Management** – keep guest records with nationality and ID details.
* **User Management** – Supabase Auth for login + role-based access control.
* **Hotel Settings** – control rules (min/max nights, guests, breakfast pricing).

This project showcases integration of **Supabase backend + React frontend** with a clean UI, authentication, and database policies.

---

## ⚙️ Project Requirements

* **Node.js** ≥ 18
* **npm** or **yarn** (package manager)
* **Supabase account** ([https://supabase.com](https://supabase.com))
* Browser (Chrome/Edge/Firefox recommended)

---

## 🗄️ Database Setup (Supabase)

1. **Create a new project** in [Supabase Dashboard](https://supabase.com/dashboard).

2. Go to **SQL Editor** and paste the provided SQL script to create tables:

   * `cabins`
   * `guests`
   * `bookings`
   * `users` (linked with `auth.users`)
   * `settings`
   * Storage bucket: `cabin-images`

3. Copy your **Project URL** and **anon/public API key** from:

   ```
   Project Settings → API → Project URL & anon key
   ```

4. Create a `.env` file inside the frontend folder and add:

   ```env
   VITE_SUPABASE_URL=your-project-url
   VITE_SUPABASE_ANON_KEY=your-anon-key
   ```

---

## 💻 Running the Project Locally

1. **Clone this repository**

   ```bash
   git clone https://github.com/your-username/the-wild-oasis.git
   cd the-wild-oasis
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Configure environment variables**

   * Create `.env` file with Supabase keys as shown above.

4. **Start the development server**

   ```bash
   npm run dev
   ```

5. Open the app in your browser:

   ```
   http://localhost:5173
   ```

---

## ✅ Features Implemented

* 📊 Dashboard with revenue & occupancy analytics
* 🛏️ Cabin management with images and discounts
* 📅 Booking management with check-in/out flow
* 👥 Guest records with IDs and nationality
* 🔐 Supabase authentication & role-based users
* ⚙️ Hotel settings management




