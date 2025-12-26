# ✨ **Resin Art Gallery**

<div align="center">

<img src="https://img.shields.io/badge/Vue.js-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white" alt="Vue.js"/>
<img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite"/>
<img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="TailwindCSS"/>
<img src="https://img.shields.io/badge/Pinia-FFE082?style=for-the-badge&logo=vue.js&logoColor=black" alt="Pinia"/>
<img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp"/>

### **A Premium Vue.js E-Commerce Platform for Luxury Resin Art** 🎨✨

**Modern Design | Interactive Galleries | WhatsApp Integration | Dark Mode**

</div>

---

## 🌐 **Live Preview**
🔗 **[Visit Resin Art Gallery](https://mahmoudnazmy.github.io/Resin-Artistry/)**  

---

## 📖 **About The Project**

**Resin Art Gallery** is a sophisticated single-page application built with Vue 3 that showcases premium handcrafted resin art creations. Designed for art collectors and enthusiasts, the platform offers an immersive shopping experience with animated galleries, real-time product filtering, and seamless WhatsApp checkout integration.

🎨 **Design Philosophy:** Luxury minimalism meets interactive user experience  
🛍️ **Purpose:** Digital gallery for artisanal resin creations with frictionless purchasing  
💫 **Vision:** Bridge the gap between traditional art galleries and digital commerce  

---

## 🔥 **Features**

✅ **Dynamic Animations** – Smooth transitions, floating elements, and interactive hover effects  
✅ **Vue 3 Composition API** – Modern, reactive architecture with clean separation of concerns  
✅ **Advanced Product Filtering** – Multi-criteria filtering with real-time updates  
✅ **Integrated WhatsApp Checkout** – Direct order placement with formatted messages  
✅ **Dark/Light Mode** – Seamless theme switching with persistent preference  
✅ **Real-time Search** – Instant product search with recent search history  
✅ **Shopping Cart System** – Pinia-powered state management with local persistence  
✅ **Responsive Design** – Mobile-first approach with adaptive layouts  
✅ **Quick View Modal** – Product preview without page navigation  
✅ **Performance Optimized** – Vite bundling with code splitting and lazy loading  

---

## 🛠️ **Built With**

<div align="center">

| Technology | Purpose |
|------------|---------|
| <img src="https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white" alt="Vue.js"/> | Progressive JavaScript framework |
| <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite"/> | Next-generation frontend tooling |
| <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white" alt="TailwindCSS"/> | Utility-first CSS framework |
| <img src="https://img.shields.io/badge/Pinia-FFE082?style=flat-square&logo=vue.js&logoColor=black" alt="Pinia"/> | State management for Vue |
| <img src="https://img.shields.io/badge/Lucide_Icons-333333?style=flat-square&logo=node.js&logoColor=white" alt="Lucide Icons"/> | Beautiful & consistent iconography |

</div>

---

## 📂 **Project Structure**
```
resin-art-gallery/
│
├── 📁 src/
│   ├── 📁 components/          # Reusable Vue components
│   │   ├── 📁 home/           # Homepage components
│   │   ├── 📁 products/       # Product-related components
│   │   ├── AppHeader.vue      # Navigation header
│   │   ├── AppFooter.vue      # Footer with developer info
│   │   ├── SearchBar.vue      # Real-time search component
│   │   └── DarkModeToggle.vue # Theme switcher
│   │
│   ├── 📁 pages/              # Vue page components
│   │   ├── HomePage.vue       # Landing page
│   │   ├── AccessoriesPage.vue # Accessories category
│   │   ├── HomeDecorPage.vue  # Home decor category
│   │   ├── ProductCategoryPage.vue # Individual category
│   │   ├── CheckoutPage.vue   # Order checkout
│   │   └── NotFoundPage.vue   # 404 page
│   │
│   ├── 📁 stores/             # Pinia state management
│   │   ├── cart.js           # Shopping cart logic
│   │   ├── products.js       # Product data & filtering
│   │   └── ui.js            # UI state (dark mode, modals)
│   │
│   ├── 📁 composables/        # Vue 3 composables
│   │   ├── useWhatsApp.js    # WhatsApp integration
│   │   ├── useAlerts.js      # Notification system
│   │   └── useFilters.js     # Product filtering logic
│   │
│   ├── 📁 utils/              # Utility functions
│   │   ├── formatters.js     # Price formatting
│   │   ├── validators.js     # Form validation
│   │   └── animations.js     # Animation helpers
│   │
│   ├── 📁 data/               # Static data
│   │   └── categories.js     # Category structure
│   │
│   └── main.js               # App initialization
│
├── index.html                # Entry point
├── vite.config.js            # Vite configuration
└── tailwind.config.js        # Tailwind configuration
```

---
## 💡 **Key Functionalities**

### 🛒 **Shopping Cart System**
- **Pinia State Management**: Centralized cart state with persistence
- **Real-time Updates**: Automatic price calculations and quantity adjustments
- **Cross-page Sync**: Consistent cart across all routes
- **Local Storage**: Cart data persists between sessions

### 🔍 **Product Discovery**
- **Advanced Filtering**: Multi-criteria filtering with instant results
- **Real-time Search**: Fuzzy search across product names and descriptions
- **Quick View**: Modal preview without navigation
- **Category Navigation**: Hierarchical browsing structure

### 📱 **Checkout Experience**
- **Form Validation**: Client-side validation with error highlighting
- **Order Summary**: Detailed breakdown with shipping calculations
- **WhatsApp Integration**: Direct order placement with formatted messages
- **Order Confirmation**: Success notifications with redirection

### 🎨 **UI/UX Features**
- **Dark Mode**: Theme switching with system preference detection
- **Animations**: Smooth transitions and interactive hover effects
- **Responsive Grids**: Adaptive layouts for all screen sizes
- **Loading States**: Skeleton loaders and progress indicators

---

## 🔧 **Technical Implementation**

### **Vue 3 Architecture**
```javascript
// Composition API Example
<script setup>
import { ref, computed } from 'vue'
import { useCartStore } from '../stores/cart'

const cartStore = useCartStore()
const itemCount = computed(() => cartStore.itemCount)
</script>
```

### **State Management with Pinia**
```javascript
// stores/cart.js
export const useCartStore = defineStore('cart', {
  state: () => ({
    items: [],
    isOpen: false
  }),
  getters: {
    itemCount: (state) => state.items.reduce((sum, item) => sum + item.quantity, 0),
    subtotal: (state) => state.items.reduce((sum, item) => sum + (item.price * item.quantity), 0)
  },
  actions: {
    addItem(product) {
      // Add to cart logic
    }
  }
})
```

### **Dynamic Filtering System**
```javascript
// composables/useFilters.js
const filteredProducts = computed(() => {
  return products.value.filter(product => {
    const matchesCategory = !selectedCategory.value || product.category === selectedCategory.value
    const matchesPrice = product.price >= priceRange.value[0] && product.price <= priceRange.value[1]
    const matchesSearch = !searchQuery.value || 
      product.name.toLowerCase().includes(searchQuery.value.toLowerCase()) ||
      product.description.toLowerCase().includes(searchQuery.value.toLowerCase())
    
    return matchesCategory && matchesPrice && matchesSearch
  })
})
```

---

## 🎯 **Use Cases**

✅ **Art Galleries** – Digital showcase for physical art collections  
✅ **Artisan Marketplaces** – Platform for handcrafted goods  
✅ **Luxury Retail** – High-end product presentation  
✅ **Subscription Boxes** – Curated art collections  
✅ **Interior Design** – Home decor product catalogs  

---

## 🏆 **Why This Project Stands Out**

💡 **Modern Tech Stack** – Vue 3 Composition API with Vite for optimal performance  
🎨 **Premium Design** – Luxury aesthetic with attention to detail  
⚡ **Performance First** – Code splitting, lazy loading, and optimized assets  
📱 **Mobile Commerce** – WhatsApp integration taps into popular messaging platforms  
🔧 **Developer Experience** – Clean architecture with reusable components  
🌙 **Accessibility** – Dark mode, keyboard navigation, and semantic HTML  

---

## 📜 **License**

Distributed under the MIT License. See `LICENSE` for more information.

---

## 🌟 **Connect With The Developer**

<div align="center">

### **Mahmoud Nazmy**
**Full-Stack Developer | Vue.js Specialist | UI/UX Enthusiast**

<a href="https://mahmoudnazmy.github.io/Portfolio/">
  <img src="https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Portfolio"/>
</a>
<a href="https://github.com/MahmoudNazmy">
  <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
</a>
<a href="https://www.linkedin.com/in/mahmoud-n/">
  <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
</a>
<a href="https://wa.me/+201093463752">
  <img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp"/>
</a>

---

### 💼 **Need a Custom E-Commerce Solution?**

I specialize in building **modern, performant, and scalable** web applications using cutting-edge technologies.

🛍️ **E-Commerce Platforms** | 🎨 **Custom UI/UX Design** | ⚡ **Performance Optimization**

**Let's transform your business with a custom digital solution!**

<a href="https://wa.me/+201093463752">
  <img src="https://img.shields.io/badge/Contact_On_WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="Contact WhatsApp"/>
</a>

</div>

---

## ⭐ **Show Your Support**

If you find this project helpful or inspiring, please give it a star! ⭐

<div align="center">

**Made with ❤️ and 🎨 by Mahmoud Nazmy**

---

**© 2025 Resin Art Gallery | All Rights Reserved**

*Bringing art and technology together in perfect harmony* ✨

<img src="https://img.shields.io/github/stars/mahmoudnazmy/resin-art-gallery?style=social" alt="GitHub Stars"/>
<img src="https://img.shields.io/github/forks/mahmoudnazmy/resin-art-gallery?style=social" alt="GitHub Forks"/>
<img src="https://img.shields.io/github/watchers/mahmoudnazmy/resin-art-gallery?style=social" alt="GitHub Watchers"/>

</div>
