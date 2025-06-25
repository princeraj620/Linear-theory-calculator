# Deployment Guide

This guide explains how to deploy the Linear Theory Calculator to various platforms.

## 🚀 GitHub Pages (Recommended)

### Automatic Deployment

The project includes GitHub Actions for automatic deployment:

1. **Push to main branch** - The workflow will automatically deploy to GitHub Pages
2. **Access your site** at: `https://princeraj620.github.io/linear-theory-calculator/`

### Manual Deployment

1. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: `gh-pages` (or `main`)
   - Folder: `/ (root)`

2. **Create gh-pages branch** (if using separate branch):
   ```bash
   git checkout -b gh-pages
   git push origin gh-pages
   ```

## 🌐 Netlify

1. **Connect your repository**:
   - Sign up/login to Netlify
   - Click "New site from Git"
   - Connect your GitHub repository

2. **Configure build settings**:
   - Build command: (leave empty)
   - Publish directory: `.`
   - Deploy!

## 🔥 Vercel

1. **Import your repository**:
   - Sign up/login to Vercel
   - Click "New Project"
   - Import your GitHub repository

2. **Configure settings**:
   - Framework Preset: Other
   - Build Command: (leave empty)
   - Output Directory: `.`
   - Deploy!

## 📦 Local Development Server

### Using Python

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

### Using Node.js

```bash
# Install serve globally
npm install -g serve

# Serve the current directory
serve .

# Or use npx
npx serve .
```

### Using PHP

```bash
php -S localhost:8000
```

### Using Live Server (VS Code Extension)

1. Install "Live Server" extension
2. Right-click on `index.html`
3. Select "Open with Live Server"

## 🐳 Docker (Optional)

Create a `Dockerfile`:

```dockerfile
FROM nginx:alpine
COPY . /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```

Build and run:

```bash
docker build -t linear-theory-calculator .
docker run -p 80:80 linear-theory-calculator
```

## 📱 Progressive Web App (PWA)

To make it a PWA, add these files:

### manifest.json
```json
{
  "name": "Linear Theory Calculator",
  "short_name": "LinearCalc",
  "description": "Network flow analysis tool",
  "start_url": "/",
  "display": "standalone",
  "background_color": "#667eea",
  "theme_color": "#4facfe",
  "icons": [
    {
      "src": "icon-192.png",
      "sizes": "192x192",
      "type": "image/png"
    }
  ]
}
```

### service-worker.js
```javascript
const CACHE_NAME = 'linear-theory-calculator-v1';
const urlsToCache = [
  '/',
  '/index.html',
  '/linear theory algorithm.html'
];

self.addEventListener('install', event => {
  event.waitUntil(
    caches.open(CACHE_NAME)
      .then(cache => cache.addAll(urlsToCache))
  );
});
```

## 🔧 Environment Variables

No environment variables are required for this static application.

## 📊 Performance Optimization

### Before Deployment

1. **Minify HTML/CSS/JS** (optional):
   ```bash
   npm install -g html-minifier cssnano uglify-js
   ```

2. **Optimize images** (if any):
   ```bash
   npm install -g imagemin
   ```

3. **Enable compression** (server-side):
   - Gzip compression
   - Brotli compression

### CDN Integration

For better performance, consider using a CDN:

- **Cloudflare**: Free CDN with caching
- **AWS CloudFront**: Global content delivery
- **Google Cloud CDN**: High-performance delivery

## 🔍 Post-Deployment Checklist

- [ ] Test all functionality
- [ ] Check mobile responsiveness
- [ ] Verify cross-browser compatibility
- [ ] Test offline functionality
- [ ] Check loading performance
- [ ] Validate HTML/CSS
- [ ] Test form submissions
- [ ] Verify error handling

## 🚨 Troubleshooting

### Common Issues

1. **404 Errors**: Ensure `index.html` is in the root directory
2. **CORS Issues**: Use a local server instead of file:// protocol
3. **JavaScript Errors**: Check browser console for errors
4. **Styling Issues**: Clear browser cache

### Debug Mode

Add this to your HTML for debugging:

```html
<script>
  // Enable debug mode
  window.DEBUG = true;
  
  // Log all calculations
  if (window.DEBUG) {
    console.log('Linear Theory Calculator loaded in debug mode');
  }
</script>
```

## 📞 Support

For deployment issues:

- Create an issue on GitHub
- Check the troubleshooting section
- Review browser console for errors
- Test with different browsers

---

Happy deploying! 🎉 