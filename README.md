# 🎂 Birthday Wish Card

A beautiful, animated birthday wish card built with **React 19 + Vite 6 + Tailwind CSS**.

## ✨ Features

- 🎬 Animated loading screen
- 💌 3D flip greeting card
- 🎮 Interactive love-themed trivia game
- 🖼️ Canvas-painted photo gallery (8 unique themes) with masonry grid
- 🔍 Fullscreen lightbox with keyboard navigation (← → Esc)
- 📸 Polaroid scroll strip
- 🎵 Web Audio API melody player
- 💕 Floating hearts background animation
- 🎉 Surprise overlay modal
- 📱 Fully responsive

## 🚀 Quick Start

### One-Click Vercel Deployment

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/your-username/birthday-wish-card)

### GitHub + Vercel Integration

[![CI](https://github.com/your-username/birthday-wish-card/workflows/CI/badge.svg)](https://github.com/your-username/birthday-wish-card/actions)
[![Deploy to Vercel](https://github.com/your-username/birthday-wish-card/workflows/Deploy%20to%20Vercel/badge.svg)](https://github.com/your-username/birthday-wish-card/actions)
[![Lighthouse](https://github.com/your-username/birthday-wish-card/workflows/Lighthouse%20CI/badge.svg)](https://github.com/your-username/birthday-wish-card/actions)

### Local Development

```bash
# 1. Install dependencies
npm install

# 2. Start dev server
npm run dev

# 3. Build for production
npm run build

# 4. Preview production build
npm run preview
```

## 🌐 Deployment

### Automatic Deployment with GitHub + Vercel

1. **Fork this repository** to your GitHub account
2. **Connect to Vercel:**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project" → Import Git Repository
   - Select your forked repository
   - Vercel will auto-detect settings and deploy

3. **Enable Automatic Deployments:**
   - Every push to `main` branch will auto-deploy
   - Pull requests will get preview deployments
   - Lighthouse audits run on every push

### Manual Vercel Deployment

1. Push your code to GitHub/GitLab/Bitbucket
2. Connect your repository to [Vercel](https://vercel.com)
3. Vercel will automatically detect the Vite configuration and deploy
4. Your site will be live at `https://your-project-name.vercel.app`

### Required GitHub Secrets

For automatic deployment, add these secrets to your GitHub repository:

- `VERCEL_TOKEN` - Your Vercel API token
- `ORG_ID` - Your Vercel organization ID  
- `PROJECT_ID` - Your Vercel project ID

### Manual Deployment

```bash
# Build the project
npm run build

# Deploy the dist/ folder to any static hosting service
```

## 🗂️ Project Structure

```
birthday-wish-card/
├── index.html                  # Vite entry point
├── package.json
├── vite.config.js
├── tailwind.config.js
├── postcss.config.js
├── public/
│   └── heart.svg               # Favicon
└── src/
    ├── main.jsx                # React root
    ├── App.jsx                 # Root component — assembles all sections
    ├── index.css               # Tailwind directives + custom CSS
    ├── data/
    │   ├── galleryData.js      # Gallery image metadata
    │   └── gameData.js         # Trivia questions & answers
    ├── utils/
    │   ├── drawPhoto.js        # Canvas painting engine (8 themes)
    │   ├── useScrollReveal.js  # IntersectionObserver scroll-reveal hook
    │   └── useMusic.js         # Web Audio API melody hook
    └── components/
        ├── Reveal.jsx          # Scroll-reveal wrapper component
        ├── Loading.jsx         # Animated loading/splash screen
        ├── FloatingHearts.jsx  # Background floating emoji hearts
        ├── MusicBtn.jsx        # Fixed music toggle button
        ├── Overlay.jsx         # Surprise fullscreen modal
        ├── Divider.jsx         # Decorative gold divider
        ├── Hero.jsx            # Hero / landing section
        ├── CardSection.jsx     # 3D flip greeting card
        ├── GameSection.jsx     # Trivia mini-game
        ├── PhotoCanvas.jsx     # Canvas element (paints theme on mount)
        ├── PhotoCard.jsx       # Single gallery card with hover effects
        ├── GalleryStrip.jsx    # Horizontal polaroid scroll strip
        ├── GallerySection.jsx  # Full gallery: grid + strip + lightbox
        ├── Lightbox.jsx        # Fullscreen image viewer
        └── FinalSection.jsx    # Closing CTA section
```

## 🚀 Getting Started

```bash
# 1. Install dependencies
npm install

# 2. Start dev server
npm run dev

# 3. Build for production
npm run build

# 4. Preview production build
npm run preview
```

## 🎨 Customisation

| File | What to edit |
|------|-------------|
| `src/data/gameData.js` | Trivia questions & answers |
| `src/data/galleryData.js` | Gallery captions, dates, themes |
| `src/components/CardSection.jsx` | Card message text |
| `src/components/Overlay.jsx` | Surprise modal message |
| `src/components/Hero.jsx` | Hero headline & subtitle |
| `tailwind.config.js` | Colour palette (`rose`, `blush`, `gold`, `deep`) |

## 🖌️ Canvas Themes

The gallery generates artwork procedurally using the HTML Canvas API:

| Theme | Description |
|-------|-------------|
| `sunset` | Gradient sky with silhouette hills & stars |
| `golden` | Warm bokeh light circles |
| `bloom` | Procedural rose flowers |
| `night` | Deep space with crescent moon |
| `stars` | Milky way with shooting star |
| `twilight` | Purple-to-rose gradient sky |
| `roses` | Multi-layered rose bursts |
| `love` | Concentric glowing heart rings |

## 🛠️ Tech Stack

- [React 19](https://react.dev/)
- [Vite 6](https://vitejs.dev/)
- [Tailwind CSS 3](https://tailwindcss.com/)
- Web Audio API (melody)
- HTML Canvas API (artwork)
- IntersectionObserver API (scroll reveals)

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details.

### Quick Contribution Steps

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'feat: add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### What We're Looking For

- 🎨 New animations and transitions
- 📱 Mobile responsiveness improvements  
- ⚡ Performance optimizations
- ♿ Accessibility enhancements
- 🧪 Test coverage
- 📚 Documentation improvements

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with ❤️ for someone special
- Inspired by modern web animation techniques
- Powered by amazing open-source tools
