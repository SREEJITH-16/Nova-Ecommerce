# 🛍️ NOVA — Modern E-Commerce Experience

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Inter&weight=800&size=32&pause=1100&color=4F8CFF&center=true&vCenter=true&width=850&lines=Welcome+to+NOVA+%F0%9F%9B%8D%EF%B8%8F;Everything+you+need.+One+place.;Discover.+Choose.+Shop.;A+modern+e-commerce+experience." alt="Animated NOVA heading">
</p>

<p align="center">
  <strong>A polished, responsive and interactive shopping experience built with modern vanilla web technologies.</strong>
</p>

<p align="center">
  <a href="https://novaecommerce-kappa.vercel.app/"><img src="https://img.shields.io/badge/%F0%9F%9A%80%20LIVE%20DEMO-Visit%20NOVA-4F8CFF?style=for-the-badge" alt="Live Demo"></a>
  <a href="https://github.com/SREEJITH-16/Nova-Ecommerce"><img src="https://img.shields.io/badge/%F0%9F%92%BB%20SOURCE-GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="Source"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?style=flat-square&logo=javascript&logoColor=111111" alt="JavaScript">
  <img src="https://img.shields.io/badge/Responsive-Yes-22c55e?style=flat-square" alt="Responsive">
  <img src="https://img.shields.io/badge/Deployment-Vercel-black?style=flat-square&logo=vercel" alt="Vercel">
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=17&pause=900&color=38BDF8&center=true&vCenter=true&width=760&lines=Explore+%E2%86%92+Filter+%E2%86%92+Choose+%E2%86%92+Cart+%E2%86%92+Checkout;Smooth+interactions.+Persistent+state.+Responsive+UI." alt="Animated feature line">
</p>

---

## 🌐 Live Demo

### **[→ Open NOVA](https://novaecommerce-kappa.vercel.app/)**

NOVA is a standalone e-commerce storefront designed to feel like a real modern shopping platform. It combines product discovery, client-side routing, filtering, search, wishlist management, a persistent cart, checkout flow and polished responsive interactions in a lightweight frontend.

---

## ✨ Highlights

- 🛍️ **25-product catalog** with categories and detailed product views
- 🔎 **Live product search** across the catalog
- 🎛️ **Filtering and sorting** for faster product discovery
- 👀 **Quick View** for browsing products without leaving the current page
- ❤️ **Wishlist** with persistent browser storage
- 🛒 **Animated cart drawer** with quantity controls and totals
- 💳 **4-step checkout experience** with validation
- 🎉 **Order confirmation** flow
- 🌓 **Light / dark mode** with persistence
- 🧭 **Client-side routing** using the History API
- 💾 **localStorage persistence** for cart, wishlist and preferences
- 📱 **Responsive design** across desktop, tablet and mobile
- ✨ **Micro-interactions, hover states and page transitions**
- ⚡ **No framework or build step required**

---

## 🎬 Experience Flow

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Inter&weight=600&size=20&pause=800&color=6366F1&center=true&vCenter=true&width=850&lines=Discover+products+%E2%86%92+Compare+options+%E2%86%92+Save+favorites;Add+to+cart+%E2%86%92+Checkout+%E2%86%92+Confirm+your+order+%E2%9C%A8" alt="Animated shopping flow">
</p>

```text
┌──────────────┐
│    HOME      │
└──────┬───────┘
       ↓
┌──────────────┐
│    SHOP      │ ← Search / Filter / Sort
└──────┬───────┘
       ↓
┌──────────────┐
│ PRODUCT PAGE │ ← Gallery / Details / Wishlist
└──────┬───────┘
       ↓
┌──────────────┐
│ CART DRAWER  │ ← Quantity / Remove / Total
└──────┬───────┘
       ↓
┌──────────────┐
│   CHECKOUT   │ ← Information / Shipping / Payment / Review
└──────┬───────┘
       ↓
┌──────────────┐
│ ORDER SUCCESS│
└──────────────┘
```

---

## 🛒 Shopping Features

### 🔎 Search, Filter & Sort

Find products quickly using live search and combine filters with sorting options to narrow the catalog.

Supported discovery tools include:

- Product search
- Category filtering
- Price filtering
- Rating filtering
- Availability filtering
- Featured sorting
- Price: low → high
- Price: high → low
- Rating
- Newest
- Discount

### ❤️ Wishlist

Save products for later and keep wishlist state between browser sessions using `localStorage`.

### 🛍️ Cart Drawer

The cart opens as a smooth side drawer, allowing users to update quantities, remove items and review totals without losing their place in the store.

### 💳 Checkout

The checkout is presented as a four-stage shopping flow:

```text
01  Information
        ↓
02  Shipping
        ↓
03  Payment
        ↓
04  Review
```

After completion, NOVA displays a dedicated order-confirmation experience.

> This is a frontend shopping flow and does not process real payments.

---

## 🧭 Client-Side Routing

NOVA uses the browser History API to provide app-like navigation without full-page reloads.

The routing architecture supports views such as:

```text
/
/shop
/product/:id
/category/:category
/wishlist
/cart
/checkout
/order-success
```

Navigation uses `pushState`, `replaceState` and `popstate`, so browser back/forward navigation remains usable.

---

## 💾 Persistent State

NOVA uses browser `localStorage` to keep important shopping preferences available after refreshes.

```text
Cart
Wishlist
Theme preference
Recent search state
```

The application also handles storage parsing defensively so malformed stored data does not break the interface.

---

## 🎨 UI & Motion

The interface is designed around a premium storefront aesthetic rather than a dashboard layout.

### Visual details

- Clean product cards
- Strong typography hierarchy
- Soft shadows and layered surfaces
- Responsive grids
- Animated buttons and controls
- Product hover interactions
- Smooth drawer and modal transitions
- Toast notifications
- Loading states
- Empty states
- Dark-mode transitions

Animations are kept lightweight and focused on `transform` and `opacity` where possible for smoother rendering.

---

## 🖼️ Product Visuals

The project currently uses original studio-style SVG product renders stored in:

```text
assets/images/p<id>.svg
```

The product artwork is generated through the project's `art()` helper and also has a fallback path when an image fails to load.

To replace the generated artwork with photography, add optimized images to `assets/images/` while keeping the corresponding product filenames.

---

## 📱 Responsive Experience

NOVA adapts across:

| Device | Experience |
|---|---|
| 🖥️ Desktop | Multi-column storefront with full navigation |
| 💻 Laptop | Flexible product grid and compact controls |
| 📱 Tablet | Responsive catalog and navigation |
| 📲 Mobile | Touch-friendly cards, menus and checkout |

The layout is designed to avoid unnecessary horizontal scrolling and keep key shopping actions easy to reach.

---

## 🌙 Dark Mode

NOVA includes a persistent light/dark theme switch.

The selected theme is saved locally so the interface remains consistent across visits.

---

## ⚡ Performance Mindset

The project is intentionally lightweight and does not require a JavaScript framework or build pipeline.

Performance-focused decisions include:

- Lazy-loaded product imagery where appropriate
- Lightweight vanilla JavaScript
- Minimal dependencies
- Efficient DOM updates
- Event-driven interactions
- CSS-based transitions
- No unnecessary runtime framework overhead

---

## 🧰 Tech Stack

| Technology | Role |
|---|---|
| **HTML5** | Semantic page structure |
| **CSS3** | Layout, responsive design, themes and animations |
| **JavaScript ES6+** | Application logic, routing and state |
| **History API** | Client-side navigation |
| **localStorage** | Persistent cart, wishlist and preferences |
| **SVG** | Product artwork and lightweight visuals |
| **Vercel** | Production deployment |

---

## 📂 Project Structure

```text
Nova-Ecommerce/
│
├── assets/
│   └── images/
│       └── p*.svg
│
├── css/
│   └── style.css
│
├── js/
│   └── app.js
│
├── index.html
├── 404.html
├── _redirects
├── vercel.json
├── .gitignore
└── README.md
```

---

## 🚀 Run Locally

Clone the repository:

```bash
git clone https://github.com/SREEJITH-16/Nova-Ecommerce.git
cd Nova-Ecommerce
```

Because client-side routes such as `/shop` need a server fallback to `index.html`, run a local static server:

```bash
npx serve -s .
```

Then open the local URL shown by the server.

---

## ☁️ Deployment

NOVA is ready for static deployment.

### Vercel

Import the repository into Vercel and use:

```text
Framework: Other
Build Command: None
Output Directory: .
```

The included `vercel.json` handles the required route fallback.

### Netlify

The included `_redirects` file provides the SPA fallback configuration.

### GitHub Pages

A `404.html` fallback is included for deep-link loading. For project-site deployments, adjust absolute asset paths or use a custom domain / user site configuration as needed.

---

## 🔗 Project Links

| Resource | Link |
|---|---|
| 🌐 **Live Website** | [novaecommerce-kappa.vercel.app](https://novaecommerce-kappa.vercel.app/) |
| 💻 **GitHub Repository** | [SREEJITH-16/Nova-Ecommerce](https://github.com/SREEJITH-16/Nova-Ecommerce) |

---

## 📋 Feature Checklist

| Feature | Status |
|---|:---:|
| Product catalog | ✅ |
| Product details | ✅ |
| Search | ✅ |
| Filtering | ✅ |
| Sorting | ✅ |
| Quick View | ✅ |
| Wishlist | ✅ |
| Cart drawer | ✅ |
| Quantity controls | ✅ |
| Checkout | ✅ |
| Order confirmation | ✅ |
| Client-side routing | ✅ |
| Browser navigation | ✅ |
| localStorage | ✅ |
| Dark mode | ✅ |
| Responsive UI | ✅ |
| Animated interactions | ✅ |
| Static deployment | ✅ |

---

## 🔮 Future Enhancements

Possible extensions for the platform include:

- Real product backend
- Authentication and user accounts
- Real payment integration
- Order history
- Product reviews from a database
- Inventory management
- Admin dashboard
- Personalized recommendations
- Product comparison
- PWA / offline support

---

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Inter&weight=700&size=20&pause=1300&color=4F8CFF&center=true&vCenter=true&width=760&lines=Discover.+Choose.+Shop.;NOVA+%E2%80%94+Everything+you+need.+One+place.;Thanks+for+visiting+NOVA+%E2%9C%A8" alt="Animated NOVA footer">
</p>

<p align="center">
  <a href="https://novaecommerce-kappa.vercel.app/"><strong>🛍️ Launch NOVA →</strong></a>
</p>
