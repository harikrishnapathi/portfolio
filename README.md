# Harikrishna Pathi — Portfolio Setup Guide

## Project Structure
```
portfolio-vercel/
├── api/
│   └── chat.js          ← Secure backend (holds your API key)
├── public/
│   └── index.html       ← Your portfolio website
├── vercel.json          ← Vercel config
├── package.json
└── README.md
```

---

## Step 1 — Get your Anthropic API Key

1. Go to https://console.anthropic.com
2. Sign up / log in (free account works)
3. Click **"API Keys"** in the left menu
4. Click **"Create Key"** → copy it (starts with `sk-ant-...`)
5. Add $5 credit — that's enough for thousands of demo uses

---

## Step 2 — Upload to GitHub

1. Go to https://github.com → **New repository**
2. Name it: `portfolio` (or anything you like)
3. Set to **Public**
4. Click **"uploading an existing file"**
5. Upload all files keeping the folder structure:
   - `api/chat.js`
   - `public/index.html`
   - `vercel.json`
   - `package.json`
6. Commit changes

---

## Step 3 — Deploy on Vercel (Free)

1. Go to https://vercel.com → Sign up with GitHub
2. Click **"Add New Project"**
3. Import your `portfolio` GitHub repo
4. Click **Deploy** (leave all settings default)
5. Wait ~1 minute for deployment

---

## Step 4 — Add your Secret API Key (IMPORTANT)

This keeps your key safe — never exposed to visitors:

1. In Vercel dashboard → your project → **Settings**
2. Click **"Environment Variables"** in left menu
3. Click **"Add New"**
4. Name: `ANTHROPIC_API_KEY`
5. Value: paste your `sk-ant-...` key
6. Click **Save**
7. Go to **Deployments** → click the 3 dots → **Redeploy**

---

## Step 5 — Your site is live! 🎉

Your URL will be: `https://your-project-name.vercel.app`

All 4 AI tools will work:
- ✅ AI Support Chatbot
- ✅ Code Generator  
- ✅ Product Description Writer
- ✅ Resume Analyzer

---

## Optional: Custom Domain

Want `harikrishna.dev` instead of `.vercel.app`?
1. Buy domain on Namecheap (~$10/year)
2. Vercel Settings → Domains → Add your domain
3. Follow DNS instructions

---

## Cost Estimate

| Service | Cost |
|---------|------|
| Vercel hosting | FREE forever |
| Anthropic API (demos) | ~$0.001 per message |
| $5 credit | ~5,000 demo messages |

---

## Need help? 
Email: Harikrishnapathi02@gmail.com
