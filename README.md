<div align="center">

# What To Eat Today · 三餐有意思

**A warm AI meal planner for recipe ideas, daily food logs and “what should I eat?” moments.**

[English](./README.md) | [简体中文](./README.zh-CN.md)

[![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev)
[![Vite](https://img.shields.io/badge/Vite-6-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vite.dev)
[![AI](https://img.shields.io/badge/AI-Gemini-F97316?style=for-the-badge)](#ai-features)
[![License](https://img.shields.io/badge/LICENSE-MIT-10B981?style=for-the-badge)](./LICENSE)

</div>

---

## What it is

The current version is a React web app focused on everyday meal decisions.

It combines:

- AI-assisted recommendations
- recipe collection
- daily meal logging
- shopping lists
- favorites
- content / image-based recipe parsing
- local fallback storage

---

## 🎬 Demo

<div align="center">

<img width="92%" alt="What To Eat Today" src="https://github.com/user-attachments/assets/5bcb3c7a-6939-4720-bb56-9a1640f97e43" />

</div>

> The repository used to target a mini-program architecture. The current codebase is React 19 + Vite; this README follows the current implementation.

---

## ⚡ Quick Start

```bash
git clone https://github.com/Dream22180971/food-menu-app.git
cd food-menu-app

npm install
npm run dev
```

Open `http://localhost:3000`.

---

## ✨ Core Experience

| Area | What it does |
|---|---|
| Home | AI meal recommendations and daily food log |
| Discovery | browse and search recipes |
| Shopping | maintain a grocery / ingredient list |
| Favorites | save recipes you want to revisit |
| AI parsing | extract recipe information from supplied content |
| Local fallback | keep basic data in `localStorage` when needed |

---

## 🧠 AI Features

The app includes AI service hooks for:

- meal recommendations
- recipe parsing
- content-assisted recipe creation

The exact AI behavior depends on the configured model/service environment.

---

## 🧭 Product Direction

The product is intentionally not just a recipe catalog. The stronger direction is:

```text
What do I have?
      ↓
What can I cook?
      ↓
What did I eat today?
      ↓
What should I buy next?
```

That turns recipes into a lightweight daily meal workflow.

---

## 🛠 Stack

```text
React 19
Vite 6
TypeScript
Motion
Firebase
Google GenAI
localStorage fallback
```

---

## 🗺 Roadmap

- [x] recipe cards and discovery
- [x] daily meal logs
- [x] favorites
- [x] shopping list
- [x] AI recommendations
- [ ] stronger ingredient recognition flow
- [ ] weekly meal planning
- [ ] nutrition summaries
- [ ] better sync / account model
- [ ] shareable recipe cards

---

## ⚠️ Current Limitations

- AI functionality depends on environment configuration
- local fallback storage is device-specific
- some older README assumptions no longer apply to the current React codebase

---

## 📄 License

[MIT](./LICENSE)

<div align="center">

**Less staring at the fridge. More actually eating well.**

</div>
