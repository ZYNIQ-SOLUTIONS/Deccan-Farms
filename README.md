# 🌿 Deccan Farms — Pune's Fresh-Cut Produce Atelier

[![Deploy Status](https://img.shields.io/badge/deployment-Netlify-00C7B7?style=flat-square&logo=netlify&logoColor=white)](https://deccanfarms.netlify.app)
[![Platform](https://img.shields.io/badge/platform-Mobile--First%20Web%20App-0E2316?style=flat-square)](https://github.com/ZYNIQ-SOLUTIONS/Deccan-Farms)
[![Purity Standard](https://img.shields.io/badge/hygiene-3--Stage%20Ozone%20Wash-34D399?style=flat-square)](https://github.com/ZYNIQ-SOLUTIONS/Deccan-Farms)
[![Zero Waste](https://img.shields.io/badge/weight-100%25%20Edible%20Net-E07A4F?style=flat-square)](https://github.com/ZYNIQ-SOLUTIONS/Deccan-Farms)
[![Coverage](https://img.shields.io/badge/service-Pune%20Metro-D4AF37?style=flat-square)](https://github.com/ZYNIQ-SOLUTIONS/Deccan-Farms)

> **"We aren't simply selling cut fruits and vegetables — we're making it easier for people to eat fresh every day."**

Deccan Farms is a mobile-first, TikTok/Reels-style web experience delivering triple ozone-washed, cold-cut vegetables, hand-peeled fruits, and artisanal chef salads across Pune. Sourced at dawn from partner farms in Mulshi, Satara, and Solapur, processed in an 18°C pharmaceutical-grade cleanroom, and dispatched chilled to Pune kitchens.

---

## ✨ Key Features & User Experience

### 1. 📱 TikTok / Reels Full-Bleed Vertical Snap Feed
- **Immersive Full-Screen Experience**: Effortless vertical swipe and snap scrolling mimicking modern short-form video feeds.
- **Dynamic Chromatic Adaptation**: Background colors and mood palettes morph smoothly (`var(--sec-bg)`) per product category as users scroll.
- **Story Progress Navigation**: Top-segmented story progress bar indicating active position across the 13 curated screens.

### 2. ⚡ Centered Sticky Action Rail
- **One-Tap Bagging**: Add items directly to your bag with real-time floating badge counters.
- **Micro-Interactions**: Floating heart animations on like, Web Share API integration with automatic clipboard fallback.
- **Deep Inspection**: Quick-access modal detailing cutting style, nutrition, preparation tips, and hygiene facts.

### 3. 🧼 4-Step Medical Cleanroom Protocol
- **01. Dawn Harvest**: Harvested and procured within 6 hours of sunrise from Mulshi and Satara farmers.
- **02. 3-Stage Ozone Bio-Wash**: Electrolytic ozone micro-bubble wash neutralizing 99.9% of surface pesticides, dirt, and microbial load without chemical residues.
- **03. 18°C Cleanroom Cut**: Processed using surgical-grade SS316 blades under temperature-regulated positive pressure to prevent cellular bruising and oxidation.
- **04. Breathable Punnets**: Sealed in food-grade, BPA-free breathable punnets that retain crisp crunch for up to 4 days refrigerated.

### 4. 🛒 Smart Fresh Bag & Instant WhatsApp Checkout
- **Dynamic Weight Toggles**: Instant price calculations for 250g, 500g, and 1kg portion sizes with MRP comparative savings.
- **Free Delivery Progress**: Interactive threshold bar tracking progress towards ₹199 free shipping.
- **Neighborhood Delivery Routing**: Pre-configured delivery slots across Pune IT & residential hubs (Koregaon Park, Baner, Kalyani Nagar, Viman Nagar, Aundh, Wakad, Hinjewadi, Kharadi, and Magarpatta).
- **1-Click WhatsApp Ordering**: Formats entire cart, delivery instructions, address, and total into a clean, ready-to-send WhatsApp message for instant concierge fulfillment.

### 5. ⏱ Interactive Kitchen Prep Time Calculator
- Dynamic weekly time-saved slider demonstrating hours saved from peeling, washing, and chopping (averaging 6.5+ hours saved weekly per household).

---

## 🥗 Curated Daily Menu

| Category | Item | Cut & Preparation | Key Benefit |
| :--- | :--- | :--- | :--- |
| **Fruits** | **Ruby Bhagwa Pomegranate Arils** | Hand-peeled intact arils | Zero bitter pith, Solapur sweet arils, zero stained fingers |
| **Vegetables** | **Cleaned & Plucked Gavran Methi** | Tender leaves only, triple-washed | 100% edible net weight, zero mud or stems, ready for kadhai |
| **Salads** | **Asian Edamame & Quinoa Bowl** | Shredded cabbage, edamame, sesame dressing | 18g plant protein, chef-crafted dressing pot included |
| **Vegetables** | **Exotic Wok Stir-Fry Medley** | Broccoli florets, zucchini batons, peppers | 4-minute wok-toss cut, high fiber & Vitamin C |
| **Fruits** | **Sun-Ripened Papaya & Pineapple** | 1-inch bite cubes | Naturally ripened, carbide-free, digestive enzymes |
| **Salads** | **Mediterranean Chickpea & Feta** | Diced English cucumber, cherry tomatoes, olives | High fiber, authentic Greek feta, vinaigrette included |
| **Vegetables** | **Pav Bhaji & Sambar Diced Mix** | Uniform diced cauliflower, carrots, peas, beans | Direct to pressure cooker, saves 20 mins of chopping |
| **Fruits** | **Chilled Kiran Watermelon & Mint** | Crisp bite-sized cubes + farm mint | Seedless, ultra-hydrating electrolyte boost |
| **Vegetables** | **Peeled Gavran Garlic (Lasun)** | Whole unblemished cloves | Unbruised, unbleached, 7-day crisp refrigerator life |

---

## 🏗 Tech Stack & Architecture

- **Core Engine**: Pure Semantic HTML5, CSS3 Custom Properties, and Modern ES6+ JavaScript (zero external framework overhead for instantaneous 60fps load and scroll performance).
- **Typography**: Google Fonts — *Cormorant Garamond* (luxury editorial display serif) paired with *Plus Jakarta Sans* (geometric clean sans-serif).
- **APIs & Browsers**:
  - `IntersectionObserver API` for slide intersection detection and dynamic background styling.
  - `CSS Scroll Snap` (`scroll-snap-type: y mandatory`) for fluid, native vertical gestures.
  - `Web Share API` (`navigator.share`) with fallback clipboard link copy.
  - `localStorage` for cart persistence, liked products, and user preferences.
- **Deployment & Hosting**: Netlify with optimized security headers (`X-Frame-Options`, `X-Content-Type-Options`, `Strict-Transport-Security`, `Permissions-Policy`), cache-control rules, and SPA redirects.

---

## 📁 Repository Structure

```
Deccan-Farms/
├── index.html       # Complete application engine (markup, styling, catalog data, UI state logic)
├── netlify.toml     # Production deployment configuration, security headers, and caching
├── _redirects       # Netlify URL rewrite rules for clean route resolution
└── README.md        # Project documentation and developer reference
```

---

## 🚀 Getting Started

### Local Development

Because Deccan Farms is built entirely with lightweight, zero-dependency web technologies, you can run it using any local HTTP static server:

```bash
# Clone the repository
git clone https://github.com/ZYNIQ-SOLUTIONS/Deccan-Farms.git
cd Deccan-Farms

# Option 1: Using Node.js npx serve
npx serve .

# Option 2: Using Python 3 built-in HTTP server
python3 -m http.server 8000

# Option 3: Using VS Code / Cursor Live Server extension
# Right click index.html -> "Open with Live Server"
```

Open your browser at `http://localhost:8000` or `http://localhost:3000`.

---

## 📦 Deployment

The project is configured for instantaneous continuous deployment with **Netlify**:

1. Link your GitHub repository to Netlify.
2. Build Settings:
   - **Base directory**: `.`
   - **Publish directory**: `.`
   - **Build command**: *(None required — pure static delivery)*
3. Netlify automatically consumes `netlify.toml` for HTTP security headers and cache policies.

---

## 📍 Pune Delivery Zones

Deccan Farms serves kitchens and corporate campuses across Pune, including:
- **East Pune**: Koregaon Park, Kalyani Nagar, Viman Nagar, Magarpatta City, Kharadi
- **West Pune**: Baner, Balewadi High Street, Aundh, Pashan
- **Tech Corridors**: Hinjewadi Phases 1–3, Wakad

---

## 📄 License & Ownership

© 2026 **Deccan Farms** (ZYNIQ SOLUTIONS). All rights reserved.
Built with dedication for healthier, effortless living in Pune.
