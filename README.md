# 🏔️ Morocco Atlas Adventure

A modern, multilingual tourism website built with **React + Vite**, showcasing Morocco’s guided tours, trekking expeditions, and adventure activities.
**Deployed at: moroccoatlasadventure.com**

## 🌍 Overview

**Morocco Atlas Adventure** is a full-featured travel website displaying:

* ✔️ City tours (Marrakech, Fez, Casablanca, Tangier)
* ✔️ Trekking expeditions (Atlas Mountains, Rif Mountains, Sahara Desert)
* ✔️ Adventure activities (4x4 tours, camel rides, quad biking, hot air ballooning…)
* ✔️ Cultural immersion experiences

The application is fully multilingual, SEO-optimized, mobile-responsive, and designed with a clean, content-first user experience.

---

# 🚀 Tech Stack

### **Frontend**

* React 18
* Vite 5
* React Router DOM
* CSS Modules

### **Internationalization**

* i18next
* react-i18next
* Language detector + HTTP backend
* Languages: **English, Spanish, Italian**

### **UI & Assets**

* Font Awesome
* Google Fonts (Montserrat)
* react-icons
* Leaflet + react-leaflet (maps)

### **SEO & External APIs**

* react-helmet-async
* Web3Forms (contact form)
* hCaptcha
* OpenStreetMap tiles

---

# 🧱 Project Architecture

```
src/
├── components/      # Shared UI components
├── features/        # Domain features (tours, trekking, gallery…)
├── pages/           # Route-level pages
├── routes/          # Routing config
├── hooks/           # Custom hooks
├── utils/           # Helpers/constants
├── styles/          # Global styles
└── i18n/            # Translation config
```

### 🏗 Key decisions

* Feature-based architecture
* Route-level **lazy loading** for performance
* Scoped CSS with modules
* Error boundaries
* Path aliases (`@components`, `@features`, …)
* SEO-first page structure

---

# ✨ Features

### 🌐 **Multilingual Support**

* Automatic language detection
* Language switcher
* All content translated dynamically

### 🗺️ **Tours & Trekking Modules**

* Detailed pages with:

  * Hero section + statistics
  * Day-by-day itinerary
  * What’s included / not included
  * High-quality image galleries

### 🖼️ **Gallery System**

* Category-based gallery
* Lightbox functionality
* Fully responsive grid

### ✉️ **Contact System**

* Form with validation
* hCaptcha bot protection
* Web3Forms API submission
* Leaflet interactive map

### 🏠 **Homepage**

* Hero banner
* About preview
* Featured tours & trekking trips
* Activities section
* Gallery preview
* Embedded contact section

---

# ⚙️ Implementation Details

### 📦 Performance

* Code splitting (React.lazy + Suspense)
* Manual vendor chunking (React, i18n, Leaflet)
* Optimized build output with Vite

### 🔐 Security

* Environment variables for API keys
* hCaptcha protection
* No sensitive data stored client-side

### ♿ Accessibility

* Semantic HTML
* ARIA labels
* Keyboard-friendly navigation

---

# 📡 Data & APIs

### **Static Data**

The project uses JavaScript files for tours, trekking trips, gallery items, etc.

Example structure:

```js
{
  id: "toubkal-7d",
  hero: {
    title: "7-Day Toubkal Summit",
    heroImg: "/images/toubkal.jpg",
    stats: [
      { label: "Duration", value: "7 Days" },
      { label: "Elevation", value: "4167m" }
    ]
  },
  journey: { ... },
  timeLine: [ ... ],
  infoCards: [ ... ]
}
```

### **External APIs**

* **Web3Forms** → form submissions
* **OpenStreetMap** → Leaflet map tiles

---

# 🛠️ Development

### **Install**

```bash
npm install
```

### **Run Dev Server**

```bash
npm run dev
```

### **Build**

```bash
npm run build
```

### **Preview Build**

```bash
npm run preview
```

### **Lint**

```bash
npm run lint
```

---

# 🚀 Deployment

* Output is a **static SPA** (`dist/`)
* Works with Netlify, Vercel, GitHub Pages
* Includes Netlify redirect rule for client-side routing:

```
/*  /index.html  200
```

### Required environment variables:

```
VITE_WEB3FORMS_KEY
VITE_HCAPTCHA_SITE_KEY
```

---

# 🔮 Future Enhancements

### Short Term

* Add testing (Jest + React Testing Library)
* WebP & lazy-loading images
* Analytics (GA4)

### Medium Term

* Headless CMS (Contentful, Strapi)
* Online booking system + payments
* User accounts + saved favorites

### Long Term

* Full backend (Express + DB)
* Mobile app (React Native)
* 360° virtual tours
* Multi-currency support

---

# 📊 Project Stats

* 50+ React components
* 10+ routes
* 100+ images
* 3 supported languages
* 8+ trekking expeditions
* Fully SEO-optimized

---

# 📌 Status
**Deployed at: moroccoatlasadventure.com**
**Production Ready**
**Last Updated: 2025**
