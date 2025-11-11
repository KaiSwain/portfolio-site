# Deploy Portfolio to Railway

## Prerequisites
- GitHub account
- Railway account (sign up at https://railway.app)

## Deployment Steps

### 1. Initialize Git Repository (if not already done)
```bash
cd /home/kaifer/workspace/portfolio-site
git init
git add .
git commit -m "Initial commit - Kai Swain Portfolio"
```

### 2. Push to GitHub
```bash
# Create a new repository on GitHub (https://github.com/new)
# Name it something like: portfolio-site

# Then push your code:
git remote add origin https://github.com/KaiSwain/portfolio-site.git
git branch -M main
git push -u origin main
```

### 3. Deploy to Railway

1. Go to https://railway.app
2. Click "Start a New Project"
3. Select "Deploy from GitHub repo"
4. Choose your `portfolio-site` repository
5. Railway will auto-detect the configuration from `railway.json`
6. Click "Deploy"

### 4. Add Custom Domain

After deployment:

1. Go to your project in Railway dashboard
2. Click on your service
3. Go to "Settings" tab
4. Scroll to "Domains" section
5. Click "Generate Domain" for a free Railway subdomain (like `your-portfolio.up.railway.app`)
6. OR click "Custom Domain" to add your own domain:
   - Enter your domain (e.g., `kaiswain.com`)
   - Add the CNAME record to your domain's DNS settings
   - Point it to the Railway domain provided

### Railway Free Tier
- $5 free credit per month
- Enough for personal portfolios
- Auto-sleeps after inactivity (wakes up instantly)

### Alternative: Use Netlify or Vercel (Even Simpler)

Both offer better free tiers for static sites:

**Netlify:**
1. Go to https://netlify.com
2. Drag and drop your portfolio-site folder
3. Get instant deployment with free SSL
4. Add custom domain in settings

**Vercel:**
1. Go to https://vercel.com
2. Import from GitHub
3. Auto-deploy on every push
4. Free custom domains and SSL

## Your Portfolio URLs
- Railway: Will be `https://your-app-name.up.railway.app`
- Custom domain: Whatever you choose (e.g., `https://kaiswain.com`)

## Environment
The portfolio uses:
- Static HTML, CSS, and JavaScript
- Python's built-in HTTP server for serving files
- No backend or database required
