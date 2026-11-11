# Bhargav Jha - Young Tech Explorer Website

A modern, sci-fi themed personal website for Bhargav Jha, an 8-year-old robotics and computer science enthusiast.

## Features

- 🎨 **Modern Sci-Fi Design** - Neon colors, grid backgrounds, particle effects
- 🤖 **Tech-Themed Animations** - Floating particles, scanlines, glow effects
- 📱 **Fully Responsive** - Works on mobile, tablet, and desktop
- ⚡ **Performance Optimized** - Built with Vite, React, and Tailwind CSS
- 🎯 **Interactive Components** - Project modals, interest tabs, timeline

## Tech Stack

- **Framework**: React 18 + TypeScript
- **Build Tool**: Vite 5
- **Styling**: Tailwind CSS 3
- **Fonts**: Orbitron, Space Grotesk, JetBrains Mono (Google Fonts)
- **Animations**: CSS animations + Canvas API

## Getting Started

### Prerequisites

- Node.js 18+
- npm or pnpm

### Installation

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Project Structure

```
src/
├── components/
│   ├── BackgroundEffects.tsx  # Canvas particle system
│   ├── Hero.tsx               # Landing hero section
│   ├── About.tsx              # About & timeline
│   ├── Interests.tsx          # Interest categories with details
│   ├── Projects.tsx           # Project showcase with modals
│   └── Footer.tsx             # Contact & social links
├── App.tsx                    # Main app component
├── main.tsx                   # Entry point
└── index.css                  # Global styles + Tailwind
```

## Customization

### Adding Bhargav's Photo

Replace the placeholder in `src/components/Hero.tsx`:

```tsx
// Replace this div:
<div className="relative w-full h-full rounded-full bg-gradient-to-br from-dark-800 to-dark-900 flex items-center justify-center border-2 border-neon-green/50 overflow-hidden">
  <span className="font-display font-bold text-5xl sm:text-6xl lg:text-7xl bg-gradient-to-r from-neon-green to-neon-blue bg-clip-text text-transparent">
    B
  </span>
</div>

// With:
<img 
  src="/bhargav.jpg" 
  alt="Bhargav Jha" 
  className="w-full h-full object-cover rounded-full"
/>
```

Then add `bhargav.jpg` to the `public/` folder.

### Updating Content

- **Personal Info**: Edit `Hero.tsx`, `About.tsx`, `Footer.tsx`
- **Interests**: Modify the `interests` array in `Interests.tsx`
- **Projects**: Update the `projects` array in `Projects.tsx`
- **Social Links**: Edit `socialLinks` in `Footer.tsx`

### Colors

Customize the neon color palette in `tailwind.config.js`:

```js
neon: {
  green: '#39ff14',    // Primary neon green
  blue: '#00ffff',     // Cyan
  purple: '#bc13fe',   // Purple
  pink: '#ff10f0',     // Magenta
}
```

## Deployment

### Vercel (Recommended)

```bash
npm run build
# Deploy the `dist` folder to Vercel
```

### Netlify

```bash
npm run build
# Deploy the `dist` folder to Netlify
```

### GitHub Pages

```bash
npm run build
# Push `dist` folder to gh-pages branch
```

## License

MIT License - Feel free to use this for your own portfolio!

---

Built with 💚 by Bhavin Jha for Bhargav Jha