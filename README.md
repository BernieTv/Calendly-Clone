# 🌟 **Meetly – A Calendly Clone**

_A full-stack scheduling app to simplify your time management._

---

## 🧭 **Overview**

Introducing **Meetly** — your intelligent, modern-day meeting scheduling solution! Inspired by **Calendly**, this clone brings seamless, efficient scheduling to life. Crafted with a robust **MERN-ish** stack: **Node.js**, **TypeORM**, **PostgreSQL**, and **React.js**, Meetly empowers users to book, manage, and sync meetings — all in a clean, responsive interface.

🧠 _Smart availability logic, timezone-aware booking, and elegant UI make Meetly the ultimate productivity ally._

---

## ✨ **Key Features**

- 🔐 **Secure Auth** — Effortless JWT-based sign-up & login
- 🗖️ **Event Creation** — Private or public events at your fingertips
- 🔗 **Sharable Links** — Share custom booking links, book instantly!
- ⏳ **Availability Control** — Define time slots, prevent double-booking
- 🌍 **Timezone Support** — Auto-detection for global coordination
- 🗕️ **Custom Calendar UI** — Built from scratch, no plugins
- 🔄 **Google Calendar Integration** — Sync with Google Meet & Calendar
- ✅ **Meeting Dashboard** — Track upcoming, past & canceled meetings
- 🧐 **Time Format Toggle** — Choose between 12h & 24h display
- 📥 **Email Notifications** — Stay in the loop with meeting alerts
- 🧹 **Modular Codebase** — Scalable and maintainable architecture
- 💻 **Tech Stack** — Node.js • TypeORM • PostgreSQL • React.js
- 🎨 **Modern UI** — Styled with TailwindCSS v4 & Shadcn UI

---

## ⚙️ **Tech Stack & Tools**

Meetly brings together the best of modern web development:

| 💻 Backend | 🌐 Frontend    | 🛠️ Dev Tools       | 🔗 Integration          |
| ---------- | -------------- | ------------------ | ----------------------- |
| Node.js    | React.js       | Vite.js            | Google Calendar API     |
| TypeORM    | TailwindCSS v4 | TypeScript         | OAuth 2.0               |
| PostgreSQL | Shadcn UI      | JWT Authentication | Google Meet Integration |

---

## 🚀 **Getting Started**

Spin up your own instance of Meetly in just a few steps:

### 🛠️ 1. Clone the Repo

```bash
git clone https://github.com/BernieTv/Calendly-Clone.git
cd Calendly-Clone
```

---

### 🔐 2. Set Up Backend Environment Variables

Navigate to the backend directory and create a `.env` file:

```bash
cd backend
touch .env
```

Add the following configuration:

```env
PORT=8000
NODE_ENV=development

DATABASE_URL="postgresql://<USER>:<PASSWORD>@<HOST>:<PORT>/<DB_NAME>"

JWT_SECRET="your_jwt_secret"
JWT_EXPIRES_IN="1d"

GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=
GOOGLE_REDIRECT_URI="http://localhost:8000/api/integration/google/callback"

FRONTEND_ORIGIN=http://localhost:5173
FRONTEND_INTEGRATION_URL=http://localhost:5173/app/integrations
```

> 🛡️ _These settings configure the server, database, authentication, and Google integrations._

---

### 🌐 3. Set Up Frontend Environment Variables

Move into the `/frontend` folder and create a `.env` file:

```bash
cd ../frontend
touch .env
```

Then add:

```env
VITE_APP_ORIGIN="http://localhost:5173"
VITE_API_BASE_URL="http://localhost:8000/api"
```

> ⚙️ _This enables the frontend to properly interact with the backend API._

---

### 📦 4. Install Dependencies

Install dependencies for both backend and frontend:

```bash
# Backend
cd ../backend
npm install

# Frontend
cd ../frontend
npm install
```

---

### ▶️ 5. Start Development Servers

```bash
# Start backend server
cd ../backend
npm run dev

# Start frontend server
cd ../frontend
npm run dev
```

- 🎯 Backend API available at: `http://localhost:8000`
- 💻 Frontend app running at: `http://localhost:5173`

---

## 🧪 **Testing & Validation**

- ✅ API tested using Postman with secured endpoints
- 🛡️ Strong schema validation with TypeORM decorators and DB constraints

---

## 🧹 **Project Structure**

### 🔹 Backend

```bash
backend/src
├── @types
├── config
├── controllers
├── database
├── enums
├── middlewares
├── routes
├── services
├── utils
└── index.ts
```

### 🔹 Frontend

```bash
frontend/src
├── assets
├── components
├── context
├── hooks
├── layout
├── lib
├── pages
├── routes
├── store
├── types
├── App.tsx
├── index.css
├── main.tsx
└── vite-env.d.ts
```

---

## 📌 **Roadmap**

- 🔔 Email & SMS notifications via Nodemailer/Twilio
- 📊 Analytics dashboard for user scheduling trends
- 👥 Team scheduling with round-robin support
- 🧹 Third-party webhooks & Zapier integration
- 📱 Improved mobile responsiveness and PWA support

---
