# 📧 Secure Mail Console

A powerful web-based email sending console built with Node.js, Express, and Nodemailer/SMTP socket routing that allows users to send bulk emails securely using Gmail SMTP. This tool provides a clean interface for sending emails to multiple recipients with real-time status updates.

---

## 🚀 Features

* Send emails using Gmail SMTP
* Bulk email sending with background batching
* Progress tracking via HTTP chunking
* Built-in Spam Protection (Cloudflare Turnstile)
* Supports HTML email content
* Secure, Serverless backend via Cloudflare Workers
* Cross-origin support using CORS
* Ready to deploy globally on Cloudflare

---

## 🛠 Tech Stack

### Frontend
* HTML5
* CSS3 (Modern Dark Theme)
* JavaScript (ES6+)

### Backend
* Cloudflare Workers (Serverless)
* `cloudflare:sockets` based SMTP Client

### Email Service
* Gmail SMTP (via App Passwords)

---

## 📂 Project Structure

```text
secure-mail-console/
│
├── public/            # Frontend files (HTML, CSS, JS)
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── worker.js          # Cloudflare Worker Backend (SMTP & Anti-Spam)
├── wrangler.json      # Cloudflare deployment configuration
├── package.json       # Project dependencies
└── README.md
