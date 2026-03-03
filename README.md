# 🚀 Task 006 – Google OAuth Authentication

## 📖 Overview

This repository contains an **Express.js** application written in **TypeScript** that demonstrates
server-side authentication using **Google OAuth 2.0** via **Passport.js**. It was developed as
part of the **Skandavel Webtech Internship** (Task 6).

The codebase is organized with a simple routing layer under `src/routes`, a Passport strategy in
`src/strategies`, and views in `src/views`. A single login page (`index.html`) allows users to initiate
a Google sign‑in and access a protected `/profile` route once authenticated.

## 🎯 Objective

The goals of this task are to:

1. Configure Passport.js with the Google OAuth 2.0 strategy.
2. Protect backend resources using session or token checks after Google sign‑in.
3. Illustrate how environment variables are used to manage sensitive credentials.

## 🛠️ Tech Stack

- **Language:** TypeScript
- **Runtime:** Node.js
- **Framework:** Express.js
- **Authentication:** Passport.js (`passport-google-oauth20`)
- **Configuration:** dotenv for environment variables
- **Development:** ts-node for running TypeScript in dev mode

## ✨ Features

- **Google OAuth Login**: Redirects to Google's consent screen and handles the callback.
- **Protected Route**: `/profile` is only accessible to authenticated users.
- **Modular Structure**: Clear separation of concerns with routes and authentication strategy.

## ⚙️ Installation & Setup

### 1. Prerequisites

- Node.js (v14+ recommended)
- A Google Cloud project with OAuth 2.0 credentials (client ID/secret).

### 2. Clone & Navigate

```bash
cd 006_Task
```

> _Note: Replace `006_Task` with your actual folder name if different._

### 3. Install Dependencies

```bash
npm install
```

### 4. Configure Environment

Create a `.env` file at the project root with the following values:

```env
PORT=3000
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
GOOGLE_CALLBACK_URL=http://localhost:3000/auth/google/redirect
```

### 5. Start Development Server

```bash
npm run start:dev
```

Visit `http://localhost:3000` and click the "Sign in with Google" button on the homepage.

## 👤 Author

**Muhilan**
_Developer @ [Skandavel Webtech](https://www.linkedin.com/company/skandavel)_
_--- [Linkedin Profile](https://www.linkedin.com/in/rcmuhilan/)_

---

_Created for learning and assessment purposes (Task 5)._
