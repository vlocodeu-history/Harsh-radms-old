# RADMS – RDBMS Desktop Application

![Electron](https://img.shields.io/badge/Electron-20232A?style=for-the-badge&logo=electron&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)

> A modern desktop-based **RDBMS management system** built with **Next.js, and Prisma ORM**.  
> Manage **customers, quotes, purchase orders, bills, and payments** — all in one place with secure authentication and PDF support.

---

## ✨ Features

- 🔐 **Authentication & Security**
  - Prisma ORM with database authentication
  - Role-based access control (RLS equivalent handled in backend logic)

- 👥 **Customer Management**
  - Add, edit, and delete customers
  - Manage billing and shipping addresses
  - Linked directly with quotes and orders

- 📑 **Quotes Management**
  - Create and edit quotes with dynamic line items
  - Support for tax, discounts, adjustments, and totals
  - Notes, terms & file attachment support
  - Stored as JSON fields for flexibility
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
- **Backend & Database Layer:** Prisma ORM + Prisma Client  
- **Database:** PostgreSQL / MySQL / SQLite (configurable in `schema.prisma`)  
- **UI Components:** shadcn/ui, lucide-react  
- **PDF Handling:** Supabase Storage (optional) / Local PDF preview 

---

## 🚀 Getting Started

### 1. Clone the Repository
```
git clone https://github.com/username/RADMS.git
cd RADMS
```
---

### 2. Install Dependencies

```
npm install
```
---

### 3. Configure Database (Prisma)

Update your `.env` file with your database connection string:
```
DATABASE_URL="postgresql://user:password@localhost:5432/radms"
```
---

Run Prisma migrations:
```
npx prisma migrate dev
```
---

Generate the Prisma Client:
```
npx prisma generate
```
---

### 4. Run the Development Server
```
npm run dev
```
---

### 5. Build the website
```
npm run build
```
---

### 📂 Project Structure
```
RADMS/
│── prisma/
│   ├── schema.prisma     # Prisma schema definition
│   ├── migrations/       # Database migrations
│── src/
│   ├── components/       # Reusable React components
│   ├── pages/            # Next.js pages (quotes, customers, etc.)
│   ├── lib/              # Prisma client, utilities
│   ├── styles/           # Tailwind and global styles
│── public/               # Static assets
│── package.json          # Dependencies & scripts
│── README.md             # Project documentation
```
---
### 📸 Screenshots (Coming Soon)
`Add screenshots of your UI here for better presentation.`

---

### ✅ Roadmap
 Add multi-user role support (Admin, Manager, Staff)

 Export quotes and invoices to PDF/Excel

 Add email notifications for quotes & PO

 Improve dashboard analytics

---

### 🤝 Contributing
Contributions are welcome!
If you’d like to improve the system, please fork the repo and submit a pull request.

---

### 📜 License
This project is licensed under the MIT License – feel free to use it in your own projects.

---

### 👨‍💻 Author
`Vlocodeu`
Built by the Developer Team with ❤️
