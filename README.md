# PJF Data & Messaging Suite

This is an **ORIGINAL** project: **PJF Data & Messaging Suite** was developed for a real client in a political marketing agency, building an automation and data-management platform for the Mexican Federal Judiciary (Poder Judicial de la Federación), helping the team organize contact data and run outreach messaging at scale. This frontend project, built from scratch with **React 18** and **TailwindCSS**, allows users to perform deep scraping of judicial profiles, process databases with gender intelligence, and manage personalized messaging campaigns via Email and WhatsApp.

The application is **fully interactive**: you can upload JSON files, edit templates in real-time with variable detection, and manage candidates through a modern, tactile interface that prioritizes operational efficiency.

<img width="781" height="631" alt="pj-scraping" src="https://github.com/user-attachments/assets/6f7de6f2-c0b6-41a4-9ec5-bb9a21601ccc" />

---

## ✨ Overview

This is not a tutorial project or a generic template. It is a **custom data engineering tool** that combines:

* **Two-Stage Data Extraction:** Interface for link scraping and deep detail collection.
* **Intelligent Processing:** Name cleaning algorithms and automatic gender detection for high-level personalization.
* **Omnichannel Messaging Editor:** Dynamic switching between Email (purple) and WhatsApp (green) modes with visual context changes.
* **Robust Data Architecture:** Blob handling for Excel and JSON export without loss of integrity.
* **High-Precision UI/UX:** Dark mode design inspired by developer tools, optimized for long work sessions.

<img width="783" height="633" alt="pj-email" src="https://github.com/user-attachments/assets/f22b68c3-24e7-4460-b69c-c6d3c549de5e" />

<img width="765" height="633" alt="pj-email-1" src="https://github.com/user-attachments/assets/da0409ad-1657-4ba8-8513-4a5e4016263b" />

<img width="777" height="631" alt="pj-whatsapp" src="https://github.com/user-attachments/assets/dccb58e5-be38-4140-9f33-ce27732923cd" />

<img width="767" height="631" alt="pj-whatsapp-1" src="https://github.com/user-attachments/assets/f3a6d7b8-0aa8-4707-8b85-d7a20ed1fe73" />

<img width="777" height="629" alt="pj-generadorvcf" src="https://github.com/user-attachments/assets/880766f9-ed6c-4b28-bacc-7916f452b561" />

---

## 🚀 Features

* ✨ **Interactive Dashboard:** Centralized management of all project phases.
* 🔍 **Integrated Scrapers:** Interface to trigger searches for ministers, magistrates, and judges.
* 📊 **Report Generator:** Dynamic conversion of JSON results to Excel files (.xlsx).
* 📥 **Data Dropzone:** File upload area with visual status feedback and type validation.
* ✍️ **Granular Personalization:** Specific modals to edit individual messages before sending.
* 🏷️ **Dynamic Tag System:** Use of variables such as `[nombre]`, `{o|a}`, and `{El|La}` for human-like communication. Template: Estimad{o|a} [nombre], le escribimos de parte de...
Output: Estimada María, le escribimos de parte de...
* 📱 **Responsive Design:** Optimized for desktop and tablets using TailwindCSS.
* 🎨 **Status Feedback:** Loading spinners, success indicators, and animated error alerts.

---

## 🛠️ Tech Stack

| Category | Technology |
| :--- | :--- |
| **Framework** | React 18 (Vite) |
| **Styling** | TailwindCSS |
| **Iconography** | Lucide React |
| **HTTP Client** | Fetch API |
| **Animations** | Tailwind Animate |
| **State Management** | React Hooks (useState, useEffect, useMemo) |
| **Deployment** | Vercel |

---

## 💻 Getting Started

### Prerequisites

* Node.js 18+
* npm or yarn
* Active Backend API (see backend repository)

### Installation

```bash
# Clone the repository
git clone https://github.com/SALVADORPOETA/Poder-judicial-frontend-sm.git

# Navigate into the project directory
cd poder-judicial-frontend-sm

# Install dependencies
npm install
```

### Environment Variables

Create a `.env.development` file in the root directory with your API URL:
```env
VITE_APP_PASSWORD=[Password]

VITE_MODO_HIBRIDO=false

VITE_API_LOCAL=http://localhost:3001
VITE_API_NGROK=https://your-link.ngrok-free.dev
VITE_API_PROD=https://your-link.vercel.app
```

Create a `.env.production` file in the root directory with your API URL:
```env
VITE_APP_PASSWORD=[Password]

VITE_MODO_HIBRIDO=true

VITE_API_LOCAL=http://localhost:3001
VITE_API_NGROK=https://your-link.ngrok-free.dev
VITE_API_PROD=https://your-link.vercel.app
```

### Development Server

```bash
npm run dev
```

The application will be available at: `http://localhost:5173`.

---

## ⚙️ Usage

1.  **Extract:** Select a PJF list (e.g., Circuit Magistrates) and download the found links.
2.  **Process:** Upload the links JSON to the "Detail Scraper" to obtain complete profiles with email and phone numbers.
3.  **Configure:** In the Messaging Service, define your template using gender and name tags.
4.  **Review:** Click on any candidate in the table to open the final personalization modal.
5.  **Send:** Toggle between WhatsApp or Email mode and trigger the bulk communication.



---

## 📂 Project Structure

```text
frontend/
├─ src/
│  ├─ components/
│  │  ├─ LinkScraper.jsx      # Phase 1: URL Extraction
│  │  ├─ DetailScraper.jsx    # Phase 2: Deep Scraping
│  │  ├─ DataDropzone.jsx     # File Ingestion
│  │  ├─ TemplateEditor.jsx   # Dynamic Template Editor
│  │  ├─ CandidatesTable.jsx  # Database Management
│  │  ├─ MessageModal.jsx     # Email Fine-tuning
│  │  └─ WhatsAppModal.jsx    # WhatsApp Fine-tuning
│  ├─ apiConfig.js            # Endpoints Configuration
│  ├─ App.jsx                 # Router and Main Layout
│  └─ main.jsx
├─ public/
├─ tailwind.config.js
└─ package.json
```

---

## 🎨 UI & UX Design

* **Channel Visual Identity:** The system automatically switches to green for WhatsApp and purple for Email to prevent human error.
* **Editing Modals:** Clean design with `monospace` typography to facilitate the review of technical texts.
* **Tactile Interactivity:** Buttons with enhanced hover states and smooth transitions.
* **Accessibility:** Use of semantic labels and high contrast for professional environments.

---

## 📌 Originality Statement

This project is **100% original**.
* No pre-made admin templates were used.
* Name and gender processing logic was independently developed.
* The entire component architecture and scraping-to-messaging flow was designed to solve a real need in the legal sector.

---

## 👨🏽‍💻 Author

**Salvador Martínez**
*Full-Stack Developer*

* **GitHub:** [SALVADORPOETA](https://github.com/SALVADORPOETA)
* **LinkedIn:** [Salvador Martínez](https://www.linkedin.com/in/salvador-martinez-sm/)

---

## ⚖️ License

This is a portfolio project created by **Salvador Martínez**.
No commercial use intended without prior consent.
All rights reserved to the author.

---

## 💡 Notes

* Designed to optimize workflows within the Federal Judiciary.
* The frontend demonstrates advanced skills in managing complex states and designing UI for productivity tools.
