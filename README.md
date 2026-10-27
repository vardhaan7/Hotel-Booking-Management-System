# The Wild Oasis – Hotel Booking Management System

## Project Description

The Wild Oasis is a full-stack hotel booking management dashboard built using React, Vite, Styled Components, and Supabase. It helps accommodation providers manage cabins, bookings, guest records, users, and hotel settings through a centralized dashboard.

### Key Features
- Dashboard with booking statistics, occupancy, and revenue overview.
- Manage cabins, including pricing, discounts, capacity, and images.
- View and manage bookings with status filters.
- Manage guest information and user roles.
- Configure booking policies and breakfast pricing.
- Supabase authentication and PostgreSQL database integration.
- Responsive user interface.

## Project Requirements

Ensure the following are installed before running the project:

- **Node.js:** Version 16 or higher
- **npm:** Node package manager
- **Git:** For cloning the repository
- **Supabase Account:** For database, authentication, and storage
- **VS Code:** Recommended code editor
- **Web Browser:** Chrome, Edge, or Firefox

## Technology Stack

- **Frontend:** React.js, Vite
- **Styling:** Styled Components
- **Backend:** Supabase
- **Database:** PostgreSQL
- **Authentication:** Supabase Auth
- **Storage:** Supabase Storage

## Database Setup

1. Create a project at [Supabase](https://supabase.com/).
2. Open the SQL Editor in your Supabase dashboard.
3. Create the following tables using the SQL schema provided in the project documentation:
   - `cabins`
   - `guests`
   - `bookings`
   - `users`
   - `settings`
4. Enable email/password authentication in Supabase.
5. Create a Storage bucket named `cabin-images` for cabin images.
6. Configure appropriate database access policies and permissions.
7. Open **Project Settings → API** and copy your project URL and publishable/anon key.

**Note:** Review the database schema and Row Level Security (RLS) policies before running the SQL, especially if using real guest data.

## How to Run the Project Locally

### 1. Clone the Repository

```bash
git clone https://github.com/aleksandromilenkov/TheWildOasis.git
cd TheWildOasis
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the project root and add your Supabase credentials:

```env
VITE_SUPABASE_URL=https://YOUR-PROJECT-REF.supabase.co
VITE_SUPABASE_ANON_KEY=YOUR_SUPABASE_ANON_KEY
```

Replace the placeholders with your actual Supabase project values. Never expose your Supabase `service_role` key in frontend code.

### 4. Start the Development Server

```bash
npm run dev
```

Open the local URL displayed in your terminal, usually:

```text
http://localhost:5173
```

## Future Enhancements

- Automated booking notifications via email and SMS.
- Enhanced guest profiles and management.
- Role-based access control for administrators and staff.
- Integration with external booking platforms.
- Advanced analytics and mobile optimization.

## Conclusion

The Wild Oasis provides a modern and customizable solution for managing hotel and cabin operations. By combining React, Vite, and Supabase, the project aims to simplify reservation management and improve operational efficiency.

---

**Note:** The repository URL above is the one referenced in the project documentation. Replace it with your own repository URL if you are using a fork.
