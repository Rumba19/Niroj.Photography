# Photographer Portfolio

A clean, professional photographer portfolio website built with Decap CMS and Netlify.

## Setup Instructions

### 1. Initialize Git Repository
```bash
cd /Users/bikramrumba/FreeLance/ClientPortfolio
git init
git add .
git commit -m "Initial commit"
```

### 2. Create GitHub Repository
- Go to github.com and create a new repository
- Push this project to GitHub:
```bash
git remote add origin https://github.com/YOUR-USERNAME/photographer-portfolio.git
git branch -M main
git push -u origin main
```

### 3. Deploy to Netlify
- Go to netlify.com
- Click "New site from Git"
- Connect your GitHub account
- Select the photographer-portfolio repository
- Deploy settings should auto-detect

### 4. Enable Netlify Identity
- In Netlify dashboard → Site settings → Identity
- Click "Enable Identity"
- Add build settings if using a static site generator

### 5. Invite Client to CMS
- In Netlify dashboard → Identity → Invite users
- Enter client's email (e.g., alex@photographer.com)
- Client receives invite email
- Client can log in at yourdomain.com/admin

## Structure

```
/
├── index.html           # Main website
├── css/style.css       # Styling
├── admin/
│   ├── config.yml      # CMS configuration
│   └── index.html      # CMS admin panel
├── assets/images/      # Image storage
├── netlify.toml        # Netlify config
└── package.json        # Project metadata
```

## Client Login

Client visits: `yourdomain.com/admin`
- Receives magic link to their email
- Clicks link → logged in
- Can edit content without code

## What Client Can Edit

- Portfolio images and descriptions
- Testimonials
- Service offerings and pricing
- About page content
- Hero section text

All changes go to GitHub automatically.

## Local Development

To test locally:
```bash
npm start
```

Then visit http://localhost:8080

## Next Steps

1. Initialize git and push to GitHub
2. Connect to Netlify
3. Enable Netlify Identity
4. Update placeholder content with real details
5. Invite client email to CMS
