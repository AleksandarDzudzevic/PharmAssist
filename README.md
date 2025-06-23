# PharmAssist – AI-Driven Loyalty App for Pharmacies 💊

PharmAssist is a cross-platform mobile loyalty solution designed to help pharmacies engage customers through automated marketing and real-time reward systems. Currently active with paying clients and estimating over 1000 active users, PharmAssist is a growing software product with real business impact slowly expanding in similar industries such as beauty salons and other areas in need for targted tailored marketing apporach.

---

## 🚀 Overview

PharmAssist enables local pharmacies to:
- Create and manage loyalty programs through a tailored cross-platform mobile app
- Allocate points to users in real-time by scanning QR codes from printed receipts
- Allow customers to redeem rewards via a dynamic loyalty store inside the app
- Automate targeted promotions through AI-enhanced workflows using purchase history and consumer behaviour

Built with scalability and automation in mind, the app currently integrates with multiple third-party tools and is generating ongoing B2B revenue.

---

## 🧠 Core Features

| Feature | Description |
|--------|-------------|
| 🎯 Real-Time Loyalty | QR code scanning syncs purchase data with user profiles instantly |
| 🏪 Loyalty Store | Dynamic, point-based reward store visible inside the mobile app |
| 🤖 Automated Campaigns | Personalized promotions sent via Viber/Email using purchase history and LLM prompts |
| 📊 Admin Dashboard | Pharmacists can upload and trigger promotions via simple forms |
| 📱 Cross-Platform App | Built in React Native and deployed to both iOS and Android |

---

## 🛠️ Tech Stack

- **Frontend:** React Native, Expo
- **Backend:** Supabase (PostgreSQL, Auth, Storage)
- **Automation:** Make.com, n8n, OpenAI, BulkGate
- **Other Tools:** FastAPI (for custom endpoints), Google Play Console, n8n (early experiments)

---

## 🔐 Why the Code is Private

PharmAssist is a proprietary business application in production use and under active development with paying pharmacy clients. The full codebase is private to protect business logic and client data.

**However**, this case study and architecture overview are shared to provide context on the engineering and business effort behind it.

---

## 📸 Screenshots

<p align="center">
  <img src="screenshots/loyalty-store.png" width="300" alt="Loyalty Store UI" />
  <img src="screenshots/qr-scan.png" width="300" alt="QR Scan Feature" />
  <img src="screenshots/admin-form.png" width="300" alt="Admin Form Example" />
</p>

---

## 🧱 Architecture Overview

```plaintext
[Mobile App (React Native)]
         |
    [Supabase Backend] <----- Pharmacist Inputs
         |
[Automation Layer: Make, n8n, LLM (2-layer gpt api calls)]
         |
[WhatsApp / SMS / Email via BulkGate API]
         |
     [End Users]
