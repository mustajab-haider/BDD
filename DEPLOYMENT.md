# 🚀 Deployment Guide

## Vercel One-Click Deployment

This project is optimized for **one-click Vercel deployment**. Follow these steps:

### Step 1: Push to GitHub
```bash
git add .
git commit -m "Ready for Vercel deployment"
git push origin main
```

### Step 2: Deploy to Vercel
1. Go to [vercel.com](https://vercel.com)
2. Click "New Project"
3. Import your GitHub repository
4. Vercel will automatically detect the settings:
   - **Framework Preset**: Vite
   - **Build Command**: `npm run build`
   - **Output Directory**: `dist`
   - **Node Version**: `18.x` or higher

5. Click "Deploy"

### Step 3: Custom Domain (Optional)
- Go to Project Settings → Domains
- Add your custom domain
- Update DNS records as instructed

## Environment Variables

Copy `.env.example` to `.env.local` and configure:

```bash
cp .env.example .env.local
```

Available environment variables:
- `VITE_BIRTHDAY_PERSON_NAME` - Person's name
- `VITE_BIRTHDAY_MESSAGE` - Custom birthday message
- `VITE_ENABLE_MUSIC` - Enable/disable music (true/false)

## Build Optimization

The project includes:
- ✅ ESBuild minification for faster builds
- ✅ Code splitting for optimal loading
- ✅ Static asset optimization
- ✅ SEO meta tags
- ✅ Proper caching headers
- ✅ Responsive design

## Troubleshooting

### Build Fails
```bash
# Clear cache and reinstall
rm -rf node_modules dist .vite
npm install
npm run build
```

### Deployment Issues
1. Check Node.js version (18.x+ required)
2. Verify all dependencies are in package.json
3. Check build logs for specific errors

### Performance Issues
- Images are optimized automatically by Vercel
- Bundle size is optimized with code splitting
- Fonts are preloaded for faster rendering

## Alternative Hosting

The build output in `dist/` can be deployed to:
- Netlify
- GitHub Pages
- AWS S3 + CloudFront
- Any static hosting service

Just upload the contents of the `dist/` folder.
