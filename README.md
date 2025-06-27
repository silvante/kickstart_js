# 🔐 NestJS + Next.js Authentication Kickstart Template

A full-stack, production-ready authentication starter built with **NestJS** (backend) and **Next.js** (frontend). It comes with **Magic Link**, **Google**, and **GitHub** authentication strategies fully integrated, secure, and scalable for modern web applications.

---

## ✨ Features

- ⚡ Magic Link login (passwordless)
- 🟢 Google OAuth2 login
- 🐙 GitHub OAuth2 login
- 🔐 JWT-based secure session handling
- 📦 Pre-configured, scalable NestJS backend
- 🌐 Next.js frontend with authentication hooks & redirects
- 🧩 Modular & extensible codebase
- ✅ Built-in input validation & error handling

---

## 🚀 Technologies

- **Backend:** [NestJS](https://nestjs.com/) with Passport.js strategies
- **Frontend:** [Next.js](https://nextjs.org/) (App Router or Pages Router)
- **Auth:** Magic link via email + OAuth2 for Google & GitHub
- **Email Provider:** Custom (sendmail, nodemailer, etc.)
- **Database:** (Plug your own, e.g., Prisma, MongoDB, or SQL)
- **Session Storage:** JWT (can be extended to use Redis or database)

---

## 🧪 .env Example (Backend)

```env
# General App Config

DATABASE_URL="postgresql://db_user:password@localhost:5432/kickstart_js"
FRONT_ORIGIN="http://localhost:3000" # frontend link
PORT=8080
JWT_SECRET="a-string-secret-at-least-256-bits-long"

# Magic Link Email Auth

MAILER_USER="no-reply@example.uz"
MAILER_PASS="Your email app password"

# Google OAuth

GITHUB_CLIENT_ID="Your github client id"
GITHUB_CLIENT_SECRET="Your github client secret"

# Google OAuth

GOOGLE_CLIENT_ID="Your google client id"
GOOGLE_CLIENT_SECRET="Your google client secret"
