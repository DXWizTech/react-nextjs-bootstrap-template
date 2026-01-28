# React + Next.js + Bootstrap (App Router) Template

![Next.js](https://img.shields.io/badge/Next.js-16-black)
![React](https://img.shields.io/badge/React-19-blue)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5-purple)
![pnpm](https://img.shields.io/badge/pnpm-10-orange)

A **working, modern example** of using **Bootstrap 5 with React and Next.js App Router**.

This repository is a **fixed and updated version** of the official Bootstrap Next.js example, rebuilt to work correctly with:

- **Next.js App Router**
- **React 19**
- **Bootstrap 5**
- **React-Bootstrap**
- **Sass**
- **pnpm**

The original Bootstrap example was built using the **Pages Router** and does not work correctly with the App Router without changes. This project shows the correct setup.

---

## ✨ Features

- ✅ Next.js **App Router** (`app/` directory)
- ✅ Bootstrap 5 with **Sass**
- ✅ React-Bootstrap components (Popover, Buttons, etc.)
- ✅ Hydration-safe layout
- ✅ Client components handled correctly
- ✅ pnpm-compatible
- ✅ Minimal and easy to extend

---

## 📦 Tech Stack

- Next.js 16+
- React 19
- Bootstrap 5
- React-Bootstrap
- Sass
- pnpm

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/DXWizTech/react-nextjs-bootstrap-template.git
cd react-nextjs-bootstrap-template
```

### 2. Install dependencies

```bash
pnpm install
```

### 3. Run the dev server

```bash
pnpm dev
```

Open:
👉 [http://localhost:3000](http://localhost:3000)

---

## 🎨 Styling Setup

Bootstrap is imported via Sass:

```scss
// styles/main.scss
@import "../node_modules/bootstrap/scss/bootstrap";
```

You can override Bootstrap variables **before** the import.

---

## 🧠 Important Notes (Read This)

### 1. App Router vs Pages Router

This project uses **App Router** (`app/`), not `pages/`.

Many older Bootstrap + Next.js examples assume the Pages Router and will break with hydration or runtime errors when used with App Router.

---

### 2. React-Bootstrap Components

Components like:

- `OverlayTrigger`
- `Popover`
- `Tooltip`
- `Modal`

**must be client components**.

Always add this at the top:

```ts
"use client";
```

Example:

```tsx
"use client";
import { OverlayTrigger, Popover, Button } from "react-bootstrap";
```

Server components cannot use `ref` or browser events.

---

### 3. pnpm + Sass

This project works correctly with `pnpm`.
Bootstrap SCSS imports use `node_modules` paths to avoid resolution issues.

---

## 🧪 What This Project Is For

- Learning Bootstrap + React in **modern Next.js**
- Starting a new project with App Router
- Reference implementation for fixing hydration issues
- Replacing outdated Bootstrap Next.js examples

---

## 📄 License

MIT — same as Bootstrap.

---

## 🙌 Credits

- Bootstrap Team (for Bootstrap & React-Bootstrap)
- Next.js Team

This repo exists to bridge the gap between **old examples** and **modern Next.js**.

---

## 👥 Created and Maintained by **DXWiz Team**

- GitHub: https://github.com/DXWizTech
- Website: https://dxwiz.com

If you find this useful, feel free to star the repo ⭐
