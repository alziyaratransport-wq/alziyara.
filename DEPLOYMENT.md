# Deployment Guide for Al Ziyara Transport Website

## Netlify Deployment (Recommended)

### Method 1: GitHub + Netlify

1. **Push to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Al Ziyara Transport Website"
   git branch -M main
   git remote add origin YOUR_GITHUB_REPO_URL
   git push -u origin main
   ```

2. **Deploy on Netlify**
   - Go to [netlify.com](https://netlify.com)
   - Click "Add new site" → "Import an existing project"
   - Connect your GitHub account
   - Select your repository
   - Build settings:
     - Build command: (leave empty)
     - Publish directory: (leave empty or use `.`)
   - Click "Deploy site"

### Method 2: Drag and Drop

1. Go to [netlify.com](https://netlify.com)
2. Click "Add new site" → "Deploy manually"
3. Drag and drop these files/folders:
   - index.html
   - css/
   - js/
   - images/
   - assets/
   - _redirects

## Files Included for Deployment

- ✅ index.html (main page)
- ✅ css/style.css (all styling)
- ✅ js/script.js (language toggle & booking)
- ✅ images/ (7 vehicle images + hero background)
- ✅ assets/ (favicon)
- ✅ _redirects (Netlify configuration)
- ✅ README.md (documentation)

## What Happens After Deployment

1. **You get a live URL** like `your-site-name.netlify.app`
2. **All features work**:
   - Language toggle (English ↔ Urdu)
   - WhatsApp booking integration
   - Email booking
   - Social media links
3. **Mobile-friendly** automatically
4. **Free SSL certificate** included

## Custom Domain (Optional)

1. In Netlify dashboard, go to "Domain settings"
2. Click "Add custom domain"
3. Enter your domain (e.g., `alziyara.com`)
4. Follow DNS configuration instructions
5. Wait for DNS propagation (usually 1-24 hours)

## Testing Before Going Live

1. **Test language toggle**: Click the language button
2. **Test booking form**: Fill all fields and click WhatsApp/Email buttons
3. **Test on mobile**: Check responsive design
4. **Test all links**: Social media links should open in new tabs

## Important Notes

- **No build process needed** - This is a static site
- **No database required** - All data is local
- **No server needed** - Runs entirely in the browser
- **Instant updates** - Push to GitHub to update live site

## Support

For deployment issues:
- Netlify Docs: https://docs.netlify.com
- Contact: alziyaratransport@gmail.com
