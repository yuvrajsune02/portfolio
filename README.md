# 🌟 Angular Project – Best Practices Showcase

This Angular application demonstrates **modern web development best practices** and coding standards.  
It serves as a reference for building scalable, maintainable, and high-performing Angular apps.

---

## 📋 Highlights

### 1️⃣ BEM Standard CSS
- Uses **Block Element Modifier (BEM)** naming convention.
- Keeps styles modular, scalable, and easy to maintain.
- Example:
  ```scss
  .card {
    &__title {
      font-size: 1.2rem;
    }
    &--highlighted {
      background-color: yellow;
    }
  }
  ```

### 2️⃣ Proper Code Comments
- Clear, meaningful inline and block comments.
- Explains the "why" behind the code, not just the "what".
- Example:
  ```ts
  // ✅ Updates user profile after successful form submission
  updateProfile(userData: UserProfile) {
    // API call to backend
    this.userService.update(userData).subscribe();
  }
  ```

### 3️⃣ Performance & Web Vitals
- **Optimized Change Detection** with `ChangeDetectionStrategy.OnPush`.
- Lazy loading for non-critical routes.
- Preloading and caching strategies.
- Measured using **Web Vitals** and Lighthouse audits.

### 4️⃣ Cross-Browser Compatibility
- Tested in:
  - ✅ Chrome
  - ✅ Firefox
  - ✅ Safari
  - ✅ Edge
- Modern CSS with graceful fallbacks for older browsers.

### 5️⃣ Angular Signals
- Implements Angular’s **Signals API** for reactive state management.
- Eliminates the need for external state libraries in small to medium apps.
- Example:
  ```ts
  // signal for storing the current theme
  theme = signal<'light' | 'dark'>('light');
  ```

### 6️⃣ Accessibility (A11y)
- Semantic HTML and ARIA attributes.
- Keyboard navigation support.
- Sufficient color contrast for readability.
- Screen reader-friendly components.

### 7️⃣ Theme Change (Light/Dark Mode)
- Toggle between **light** and **dark** themes.
- Theme preference stored in **localStorage** for persistence.
- SCSS variables used for theme colors.

### 8️⃣ Layout Change
- Switch between **grid view** and **list view** layouts.
- Fully responsive and mobile-friendly design.
- Layout choice remembered for user sessions.

---

## 🚀 Getting Started

### Prerequisites
- **Node.js** (v18+)
- **Angular CLI** (latest)

### Installation
```bash
git clone <your-repo-url>
cd <project-folder>
npm install
```

### Development Server
```bash
npm start
```
Runs the app in dev mode at `http://localhost:4200/`.

---

## 🛠 Available Scripts

| Command            | Description                                     |
| ------------------ | ----------------------------------------------- |
| `npm start`        | Start the dev server                            |
| `npm run build`    | Build the project for production                |
| `ng lint`          | Run ESLint checks                               |
| `npm run format`   | Format code using Prettier                      |
| `ng test`          | Run unit tests                                  |

---

## 📦 Folder Structure
```
src/
 ├── app/
 │    ├── components/     # Reusable UI components (BEM standard)
 │    ├── services/       # API calls, Angular Signals state
 │    ├── layouts/        # Grid/List layouts
 │    ├── themes/         # Light/Dark theme styles
 │    └── core/           # App-wide configuration and utilities
 ├── assets/              # Images, icons, fonts
 ├── styles/              # Global SCSS with BEM structure
```

---

## 📊 Performance Monitoring
- **Web Vitals** metrics tracked for:
  - Largest Contentful Paint (LCP)
  - First Input Delay (FID)
  - Cumulative Layout Shift (CLS)
- Performance tested using:
  - Lighthouse
  - Chrome DevTools

---

## 📄 License
This project is licensed under the **MIT License**.
