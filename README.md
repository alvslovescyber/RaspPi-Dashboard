
# GlassPi Dashboard

*A unified, local-first personal dashboard powered by Vue 3*

![GlassPi Dashboard – Home]

GlassPi is a **self-hosted personal dashboard** designed to run locally (Raspberry Pi, desktop, or server) and sync everything you care about in one place — music, activity, tasks, weather, and AI-powered suggestions.

The goal is simple:
**clone the repo → add API keys → everything works flawlessly.**

No fake data. No broken states. No waiting around.

---

## ✨ Features

* 🎵 **Spotify – Now Playing**

  * Real-time playback status
  * Album art, progress, controls
  * Clean empty states when not connected

* 🏃 **Strava – Activity & Health**

  * Weekly running totals & goals
  * Steps, calories, activity summaries
  * Single-source health data (no Apple Health required)

* 📖 **Daily Reading**

  * Daily verse + recent history
  * Progress tracking
  * Clean completion flow

* ✅ **Tasks**

  * Today / Upcoming / Completed
  * Minimal, distraction-free layout

* 🤖 **AI Suggestions**

  * Scheduled or manual generation
  * Works instantly after API key is added
  * Graceful error handling & empty states

* 🌦 **Weather**

  * Location-based via Open-Meteo
  * Auto-refresh + manual refresh
  * Unit selection (°C / °F)

---

## 🧱 Tech Stack

* **Vue 3** (Composition API + `<script setup>`)
* **TypeScript**
* **Vite**
* **Local-first storage** (designed to sync immediately once keys are added)
* **Electron / Pi-friendly runtime** (no cloud dependency)

---

## 🔑 Configuration Philosophy

GlassPi does **not** ship with fake placeholders.

* No Spotify UI unless Spotify is connected
* No AI suggestions unless an OpenAI key is present
* No health data unless Strava is connected

Once you enter your API keys:

> **Everything syncs automatically and stays in sync.**

All configuration is done via the **Settings UI** — no `.env` editing required.

---

## ⚙️ Setup

### 1. Clone the repo

```bash
git clone https://github.com/your-username/glasspi-dashboard.git
cd glasspi-dashboard
```

### 2. Install dependencies

```bash
npm install
```

### 3. Run locally

```bash
npm run dev
```

### 4. Open Settings → Integrations

Add your API keys for:

* Spotify
* Strava
* OpenAI (for suggestions)

That’s it.
The dashboard will immediately populate with real data.

---

## 🧠 TypeScript & Vue Notes

This project uses **Vue 3 `<script setup>` SFCs**.

Recommended IDE setup:

* **VS Code**
* **Volar**
* **TypeScript Vue Plugin (Volar)**

### Type checking

TypeScript doesn’t understand `.vue` files by default, so this project uses:

* `vue-tsc` instead of `tsc`



