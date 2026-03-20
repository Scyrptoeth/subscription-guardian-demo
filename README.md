<div align="center">

# 🛡️ Subscription Guardian

**An AI agent that finds every subscription hiding in your Gmail — built with a single prompt.**

[![Live Demo](https://img.shields.io/badge/Live_Demo-Visit_Now-00ED64?style=for-the-badge&logo=github)](https://scyrptoeth.github.io/subscription-guardian-demo/)
[![Built With](https://img.shields.io/badge/Built_With-Adaptive_AI-006CFA?style=for-the-badge)](https://adaptive.ai)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](#license)

<br/>

<img src="https://img.shields.io/badge/Gmail_Scanner-Active-22C55E?style=flat-square&logo=gmail" /> <img src="https://img.shields.io/badge/Google_Sheets-Synced-22C55E?style=flat-square&logo=googlesheets" /> <img src="https://img.shields.io/badge/Calendar_Alerts-Created-22C55E?style=flat-square&logo=googlecalendar" /> <img src="https://img.shields.io/badge/Weekly_Reports-Sending-22C55E?style=flat-square&logo=minutemailer" />

</div>

---

## The Problem

The average person wastes **$133/month** on forgotten subscriptions. Charges pile up silently in your inbox, hit your bank account, and you never notice — until it's too late.

**Subscription Guardian solves this with zero code and zero configuration.** One natural-language prompt into [Adaptive AI](https://adaptive.ai) created a fully autonomous agent that runs 24/7.

---

## What It Does

```
One prompt → Full automation pipeline
```

| Component | Function |
|-----------|----------|
| 📧 **Gmail AI Scanner** | Scans the last 30 days of email for subscription, invoice, and payment messages |
| 📊 **Auto Google Sheet** | Creates & maintains "Subscription Tracker" with 8 columns, sorted by due date |
| 📅 **Calendar Reminders** | Adds Google Calendar events 3 days before each payment |
| 📬 **Weekly Email Digest** | Monday 8 AM summary — total costs, upcoming payments, new detections |
| ⏰ **Daily Cron Job** | Runs every day at 8:00 AM (Jakarta time), zero human intervention |

---

## The Prompt

This is the **entire prompt** that built the full agent — nothing else:

> *Build me a "Subscription Guardian" agent. Every morning at 8:00 AM Jakarta time, scan my Gmail inbox for subscription, invoice, and payment emails. Extract service name, dates, amount, currency, and billing frequency. Organize into a Google Sheet called "Subscription Tracker". Add Calendar reminders 3 days before each due date. Send a weekly Monday summary email with totals.*

That's it. Adaptive AI handled the rest.

---

## Real Results

The agent scanned a real Gmail inbox and found:

| Service | Amount | Frequency | Status |
|---------|--------|-----------|--------|
| Zoom #1 | $80.13 | Monthly | ✅ Active |
| Zoom #2 | $80.13 | Monthly | ✅ Active |
| Netflix | $20.00 | Monthly | ✅ Active |
| Academia | $0.99 | Monthly | ✅ Active |
| **Total** | **$181.25/mo** | | |

> **$181.25/month** in subscriptions found and tracked automatically.

---

## Architecture

```
Gmail Inbox
    │
    ▼
┌─────────────────────┐
│  Adaptive AI Agent   │
│  (Daily 8AM Cron)    │
└─────────┬───────────┘
          │
    ┌─────┼──────────┬──────────────┐
    ▼     ▼          ▼              ▼
 📧 AI   📊 Google   📅 Calendar   📬 Weekly
Extract   Sheet      Reminders     Summary
          Sync       (3-day prior) Email
```

**4 Google integrations working together:**
Gmail Read + Send → Google Sheets → Google Calendar — seamlessly connected through Adaptive AI.

---

## Live Demo

👉 **[scyrptoeth.github.io/subscription-guardian-demo](https://scyrptoeth.github.io/subscription-guardian-demo/)**

The interactive demo includes 9 slides with:

- Glassmorphic UI showcasing the full agent pipeline
- Real subscription data extracted from Gmail
- System status dashboard (all 6 components verified live)
- Keyboard navigation (← → arrows, spacebar, or autoplay)

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| AI Agent | [Adaptive AI](https://adaptive.ai) — natural language to full automation |
| Data Source | Gmail API (AI-powered email parsing) |
| Storage | Google Sheets ("Subscription Tracker") |
| Scheduling | Google Calendar + Cron (8 AM daily / Monday weekly) |
| Notifications | Gmail Send (weekly digest email) |
| Demo Frontend | Vanilla HTML/CSS/JS with glassmorphic design |
| Hosting | GitHub Pages |

---

## Why This Matters

- **Real problem** — subscription waste is a universal pain point
- **Single prompt** — no code, no configuration, no technical knowledge required
- **Fully autonomous** — set it once, it runs forever
- **Real data** — not a mockup; the agent scanned an actual inbox
- **4 Google services orchestrated** — from one sentence of plain English

---

## Getting Started

Want to build your own? Go to [adaptive.ai](https://adaptive.ai) and type a prompt. That's literally it.

---

## Competition Entry

🏆 This project was built for the **Adaptive AI Launch Week Competition** — demonstrating the best real-world use case powered by Adaptive AI.

---

## License

MIT — feel free to fork, remix, and build your own version.

---

<div align="center">

**Built with ❤️ using [Adaptive AI](https://adaptive.ai)**

*One prompt. Built in minutes. Saves money forever.*

</div>
