# 🐾 PDX Sitters - Automation Engine

A full-stack booking system designed to streamline childcare and pet-sitting requests in Portland, OR. This project automates the transition from a client request to a confirmed calendar event.

## 🚀 How It Works
1. **Frontend:** A responsive UI built with **Tailwind CSS** hosted on GitHub Pages.
2. **API Layer:** A **Node.js** server using **Express** hosted on Render.
3. **Database:** A **NoSQL** data store using **MongoDB Atlas** and **Mongoose** to archive booking history.
4. **Automation:** Integrates with **Google Calendar API** (via Service Accounts) and **SendGrid** to handle scheduling and notifications.

## 🛠️ Tech Stack
- **Language:** JavaScript (ES6+)
- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Cloud)
- **Styling:** Tailwind CSS
- **Integrations:** Google Cloud Platform, Nodemailer, SendGrid

## 🧠 Key Features
- **Auto-Scheduling:** Directly injects bookings into the provider's Google Calendar.
- **Async Processing:** Uses `async/await` to handle database writes and API calls simultaneously.
- **Fail-Safe Logic:** Wrapped in `try/catch` blocks to ensure a single API failure (like a timeout) doesn't crash the entire booking process.
- **Live Monitoring:** Connected to Render logs for real-time debugging.