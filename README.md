# 🛍️ Nuxt E-Commerce Landing Page

This project is a **Front-end Trainee Test Case** developed to demonstrate modern front-end development skills. It is a fully responsive e-commerce landing page built with **Nuxt 3 (Vue.js)**, utilizing a mobile-first approach and modern CSS techniques.

🔗 **Live Demo:** [https://nuxt-ecommerce-landing-pagee.vercel.app](https://nuxt-ecommerce-landing-pagee.vercel.app)

---

## 🚀 Features

### Core Requirements
- **Nuxt 3 Framework:** Built with the latest Vue.js framework.
- **API Integration:** Fetches "Featured Products" dynamically from `dummyjson.com`.
- **Mobile First & Responsive:** Fully optimized for mobile, tablet, and desktop screens.
- **Component-Based Architecture:** Clean and reusable components (Hero, ProductCard, Footer, etc.).
- **Modern Styling:** Used CSS Grid and Flexbox for layout, with glassmorphism and hover effects.

### Bonus Features
- **Checkout Page:** A dedicated route for the checkout process.
- **State Management (Cart Logic):**
  - Global cart state using Nuxt Composables (`useState`).
  - **Add to Cart:** Increases quantity if the item exists, adds new if not.
  - **Remove Item:** Allows users to remove items from the checkout summary.
  - **Dynamic Totals:** Real-time calculation of Subtotal and Total prices.
- **Product Carousel:** Horizontal scrolling list for featured products with navigation buttons.

---

## 🛠️ Tech Stack

- **Framework:** [Nuxt 3](https://nuxt.com)
- **Language:** JavaScript / Vue.js
- **Styling:** Scoped CSS (Custom implementation, no external UI libraries used)
- **API:** [DummyJSON](https://dummyjson.com/)
- **Deployment:** Vercel

---

## 📂 Project Structure

```bash
.
├── components/
│   ├── AppHeader.vue       # Navigation, Search, and dynamic Cart Badge
│   ├── AppFooter.vue       # Newsletter and Site Links
│   ├── HeroSection.vue     # "Sephora-style" Intro Banner
│   ├── ProductCard.vue     # Reusable Product Component
│   ├── CategorySection.vue # Featured Categories Grid
│   ├── CampaignSplit.vue   # Gift Week & Special Sets Banners
│   └── PromoBanner.vue     # Blue Discount Banner
├── composables/
│   └── states.js           # Global State for Cart Management
├── pages/
│   ├── index.vue           # Homepage (Landing)
│   └── checkout.vue        # Checkout Page (Form & Summary)
└── app.vue                 # Main Layout Wrapper




# Nuxt Minimal Starter

Look at the [Nuxt documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

## Setup

Make sure to install dependencies:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install

# bun
bun install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm dev

# yarn
yarn dev

# bun
bun run dev
```

## Production

Build the application for production:

```bash
# npm
npm run build

# pnpm
pnpm build

# yarn
yarn build

# bun
bun run build
```

Locally preview production build:

```bash
# npm
npm run preview

# pnpm
pnpm preview

# yarn
yarn preview

# bun
bun run preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.
