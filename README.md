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
PORT=3000
JWT_SECRET=a-strong-random-secret-key
JWT_EXPIRES_IN=1d

# Magic Link Email Auth
EMAIL_FROM=no-reply@example.com
EMAIL_HOST=smtp.example.com
EMAIL_PORT=587
EMAIL_USER=your-email-user
EMAIL_PASS=your-email-password
MAGIC_LINK_EXPIRATION_MINUTES=15
MAGIC_LINK_FRONTEND_URL=http://localhost:3001/auth/magic/callback

# Google OAuth
GOOGLE_CLIENT_ID=your-google-client-id
GOOGLE_CLIENT_SECRET=your-google-client-secret
GOOGLE_CALLBACK_URL=http://localhost:3000/auth/google/callback

# GitHub OAuth
GITHUB_CLIENT_ID=your-github-client-id
GITHUB_CLIENT_SECRET=your-github-client-secret
GITHUB_CALLBACK_URL=http://localhost:3000/auth/github/callback

# (Optional) Frontend URL for CORS and redirects
FRONTEND_URL=http://localhost:3001
