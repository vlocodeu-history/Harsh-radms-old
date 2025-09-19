# RADMS – RDBMS Desktop Application

RADMS is a **desktop-based RDBMS management system** built with **Electron, Next.js, and Supabase**.  
It provides a modern and user-friendly interface for managing **customers, quotes, purchase orders, bills, and payments** — all in one place.  

---

## ✨ Features

- 🔐 **Authentication & Security**
  - Supabase authentication
  - Row-Level Security (RLS) for user-specific data access

- 👥 **Customer Management**
  - Add, edit, and delete customers
  - Manage billing and shipping addresses
  - Linked directly with quotes and orders

- 📑 **Quotes Management**
  - Create and edit quotes with dynamic line items
  - Support for tax, discounts, adjustments, and totals
  - Notes, terms & file attachment support
  - JSONB-based storage for flexibility
  - Quote detail tabs with PDF preview and download

- 📦 **Purchase Orders**
  - Add and edit purchase orders with delivery address support
  - Dynamic item handling with auto-calculation
  - Linked to bills and payments
  - Status tracking (open/closed)

- 🧾 **Bills**
  - Bill creation and management
  - Automatic PDF generation & preview inside the app
  - Linked with payments for clear traceability

- 💳 **Payments**
  - Record payments against bills
  - Support for multiple methods (Cash, UPI, Card, etc.)
  - Auto-updates purchase order status when fully paid

- 📊 **Reports & Tracking**
  - Dashboard for quick overview
  - Status indicators (e.g., PO closed in green when paid)
  - Organized tabs for each entity (Customers, Quotes, PO, Bills, Payments)

---

## 🛠️ Tech Stack

- **Frontend & Desktop App:** Electron + Next.js + React + TailwindCSS  
- **Database & Backend:** Supabase (Postgres with JSONB support)  
- **UI Components:** shadcn/ui, lucide-react  
- **PDF Handling:** Supabase Storage + PDF preview  

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/username/RADMS.git
cd RADMS

---

### 2. Install Dependencies
```bash

bash
Copy code
npm install
3. Configure Supabase
Create a project on Supabase

Add your SUPABASE_URL and SUPABASE_ANON_KEY in a .env.local file:

env
Copy code
NEXT_PUBLIC_SUPABASE_URL=your-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-key
4. Run the Development Server
bash
Copy code
npm run dev
5. Build the Desktop App
bash
Copy code
npm run build
npm run electron
📂 Project Structure
php
Copy code
RADMS/
│── src/
│   ├── components/      # Reusable React components
│   ├── pages/           # Next.js pages (quotes, customers, etc.)
│   ├── lib/             # Supabase client and helpers
│   ├── styles/          # Tailwind and global styles
│── public/              # Static assets
│── package.json         # Dependencies & scripts
│── README.md            # Project documentation
📸 Screenshots (Coming Soon)
You can add screenshots of your UI here for better presentation.

✅ Roadmap
 Add multi-user role support (Admin, Manager, Staff)

 Export quotes and invoices to PDF/Excel

 Add email notifications for quotes & PO

 Improve dashboard analytics

🤝 Contributing
Contributions are welcome!
If you’d like to improve the system, please fork the repo and submit a pull request.

📜 License
This project is licensed under the MIT License – feel free to use it in your own projects.

👨‍💻 Author
Vlocodeu
Built by the Engineering Team with ❤️
