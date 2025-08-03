# 🎟️ TicketBaba

A blazing-fast, modern ticket booking platform built with **Next.js**, **Supabase**, and **ShadCN UI** — supporting real-time availability, seamless checkout, secure payments, and rich event management.

![Banner](https://yourdomain.com/banner.png) <!-- Optional: Replace with your real image -->

---

## 🚀 Features

- 🎫 Dynamic ticket categories & stock management
- 🛒 Intelligent cart with session-based persistence
- 💳 Payment gateway integration (AamarPay)
- 📦 Auto-expiring reservations & free-ticket handling
- 📊 Admin dashboard with charts & order analytics
- 🔐 Role-based access control (RBAC)
- ✍️ Rich text editor for event descriptions
- 🖼️ Image uploads with Supabase Storage
- 📥 CSV/Excel export for orders
- 🧾 PDF invoice/ticket generation with `puppeteer`

---

## 🖥️ Tech Stack

| Frontend    | Backend      | Database     | UI/UX         | Payments     |
|-------------|--------------|--------------|----------------|---------------|
| Next.js 14  | Supabase Edge Functions | PostgreSQL | TailwindCSS + ShadCN | AamarPay (Bangladesh) |
| TypeScript  | Supabase Auth | Row-Level Security (RLS) | @react-pdf/renderer | Stripe (coming soon) |

---

## 📸 Screenshots

| Home Page | Checkout |
|-----------|----------|
| ![Home](https://yourdomain.com/home.png) | ![Checkout](https://yourdomain.com/checkout.png) |

---

## 🛠️ Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/ticketbaba.git
cd ticketbaba
````

### 2. Install dependencies

```bash
npm install
# or
yarn
```

### 3. Setup environment variables

Create a `.env.local` file and configure:

```env
NEXT_PUBLIC_SUPABASE_URL=...
SUPABASE_SERVICE_ROLE_KEY=...
NEXT_PUBLIC_SUPABASE_ANON_KEY=...
AAMARPAY_STORE_ID=...
AAMARPAY_SIGNATURE_KEY=...
```

> 🔐 Make sure to **never expose** your service role key on the client side.

---

### 4. Run locally

```bash
npm run dev
# or
yarn dev
```

---

### 5. Supabase Setup

* Import the `schema.sql` or use the provided migration file
* Enable RLS and configure policies
* Set up storage buckets (`slideshow`, `event-images`, etc.)

---

## 🧪 Testing

```bash
npm run test
# Optional: Add Playwright / Vitest / Cypress later
```

---

## 📦 Folder Structure

```
├── app/
│   ├── api/checkout/...
│   ├── (admin)/...
│   ├── (public)/...
├── components/
│   ├── ui/
│   ├── admin/
│   └── public/
├── lib/
│   ├── supabase/
│   ├── utils/
│   └── validators/
├── types/
├── hooks/
├── styles/
└── ...
```

---

## 🙌 Contributing

Pull requests and stars are welcome!
If you find a bug or want to add a feature, feel free to open an issue.

---

## 📜 License

[MIT](LICENSE)

---

## 📞 Contact

* Author: **Sarker Ayon**
* Project: [TicketBaba](https://github.com/yourusername/ticketbaba)
* Email: [your@email.com](mailto:your@email.com)
* Twitter: [@thenicedev](https://twitter.com/thenicedev)
* Gravatar: [gravatar.com/muktaranikha](https://gravatar.com/muktaranikha)

---

> “Where events go big and tickets go fast — TicketBaba, your ultimate ticketing solution.” 🎉
