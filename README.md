# the website

A personal portfolio built using **Svelte** and **Tailwind CSS**, designed to showcase my projects, skills, and growth as a developer. The site includes subtle animations and interactive visuals to keep the experience clean yet engaging.

🔗 **Live Site**: [pranjalkumar.com](https://pranjalkumar.com)

---

## 🧰 Tech Stack

- **Svelte** – component-based, reactive frontend framework  
- **Tailwind CSS** – utility-first styling framework  
- **JavaScript**, **HTML**, **CSS**

---

## ✨ Features

- Responsive layout with Tailwind  
- Lightweight, fast-loading architecture via SvelteKit  
- Custom **particle effect** built in JavaScript  
- Fully modular structure for easy expansion  
- Built for continuous iteration as my skills grow

---

## 🛠️ Setup Instructions (for Devs)

This portfolio isn’t designed for others to clone/run — but if you *do* want to explore or build from it:

### 📦 Install dependencies
```bash
npm install
````

### 🔨 Build

```bash
npm run build
```

> Or use `npm run dev` during development.

---

## ⚙️ Tailwind Integration (Manual Setup Steps)

> If you're setting up your own SvelteKit + Tailwind stack, here's how this one was configured:

1. Create your SvelteKit project:

   ```bash
   npx create-svelte my-project
   cd my-project
   ```

2. Install Tailwind:

   ```bash
   npm install tailwindcss @tailwindcss/vite
   ```

3. Configure Vite:

   ```ts
   // vite.config.ts
   import { defineConfig } from 'vite';
   import { sveltekit } from '@sveltejs/kit/vite';
   import tailwindcss from '@tailwindcss/vite';

   export default defineConfig({
     plugins: [tailwindcss(), sveltekit()]
   });
   ```

4. Create and import Tailwind CSS:

   * `src/app.css`:

     ```css
     @import "tailwindcss";
     ```
   * `src/routes/+layout.svelte`:

     ```svelte
     <script>
       import "../app.css";
     </script>
     <slot />
     ```

---

## 🔭 Future Plans

* Add a contact form for direct reach-outs
* Continue evolving content & design as I grow

---

## 📄 License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).

© Pranjal

```

---

let me know if you want this turned into a file or want to add visuals/badges. also, congrats — this is a clean, smart first portfolio. solid foundations.
```
