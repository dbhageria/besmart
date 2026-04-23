# BeSmart Finance — Vercel Deployment Guide

**Smarter Finance. Better Future.**

---

## 🚀 Deploy to Vercel in 5 Minutes

### What you need
- A computer (Mac or Windows)
- Internet connection
- Free GitHub account → github.com
- Free Vercel account → vercel.com

---

## Step 1 — Install Node.js
Download and install from: **https://nodejs.org** (click "LTS" version)

Verify it worked — open Terminal (Mac) or Command Prompt (Windows) and type:
```
node --version
```
Should show something like `v18.x.x` ✅

---

## Step 2 — Install Vercel CLI
In your Terminal / Command Prompt:
```
npm install -g vercel
```

---

## Step 3 — Set up the project
Open Terminal, navigate to this folder, then run:
```
npm install
```
This downloads React and all dependencies (~2 minutes, one time only).

---

## Step 4 — Test it locally first
```
npm start
```
This opens **http://localhost:3000** in your browser — the full site running on your computer.
Press `Ctrl+C` to stop it when done.

---

## Step 5 — Deploy to Vercel
```
vercel
```
First time: it will ask you to log in — follow the prompts.

Answer the questions:
- **Set up and deploy?** → Y
- **Which scope?** → Your name/account
- **Link to existing project?** → N
- **Project name?** → besmartfinance (or any name)
- **Directory?** → ./ (just press Enter)

✅ Done! You get a URL like: **https://besmartfinance-abc123.vercel.app**

---

## Step 6 — Connect your domain besmartfinance.com.au

1. Go to **vercel.com** → your project → **Settings** → **Domains**
2. Type: `besmartfinance.com.au` → Add
3. Vercel shows you 2 DNS records to add
4. Log in to your domain registrar (where you bought besmartfinance.com.au)
5. Add those DNS records
6. Wait 5–30 minutes for DNS to update
7. Your site is live at besmartfinance.com.au with free SSL ✅

---

## Updating the site in future

After making changes to `src/App.jsx`:
```
vercel --prod
```
That's it — new version live in ~60 seconds.

---

## File structure
```
besmart_vercel/
├── public/
│   └── index.html          ← HTML shell (don't edit)
├── src/
│   ├── index.js            ← Entry point (don't edit)
│   └── App.jsx             ← THE FULL WEBSITE (edit this)
├── package.json            ← Project config
├── vercel.json             ← Vercel settings
├── .gitignore              ← Files to ignore
└── README.md               ← This file
```

---

## Need help?
Contact Abhishek or your developer — share this README and the folder.

**Vercel docs:** https://vercel.com/docs
**Node.js:** https://nodejs.org
