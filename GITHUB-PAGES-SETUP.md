# Le Noir Live — GitHub Pages Setup

**Goal:** Host these three pages independently so WordPress rollbacks can't touch them.

## Quick Setup (3 steps)

### 1. Create a GitHub repo
- Go to github.com and create a **new public repository**
- Name: `le-noir-live` or `lenoirsg.github.io` (if you want the shorter URL)
- Make it **public** (required for free GitHub Pages)

### 2. Push these files
Run these commands in your terminal:

```bash
cd /path/to/le-noir-live
git init
git add .
git commit -m "Le Noir Live pages"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/le-noir-live.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your actual GitHub username.

### 3. Enable GitHub Pages
- Go to your repo → **Settings** → **Pages**
- Source: **main** branch
- Save

## You'll get a live URL

**If repo name is `le-noir-live`:**
- Guest page: `https://YOUR-USERNAME.github.io/le-noir-live/guest.html`
- Dashboard: `https://YOUR-USERNAME.github.io/le-noir-live/dashboard.html`
- Console: `https://YOUR-USERNAME.github.io/le-noir-live/console.html`

**If repo name is `lenoirsg.github.io`:**
- Guest page: `https://lenoirsg.github.io/guest.html`
- Dashboard: `https://lenoirsg.github.io/dashboard.html`
- Console: `https://lenoirsg.github.io/console.html`

## Then update WordPress links

Update the QR code and any links in your WordPress site to point to the new GitHub Pages URLs instead of the old WordPress pages.

## Future updates

To update any page, edit the file locally, commit, and push:

```bash
git add .
git commit -m "Update guest page"
git push
```

Live in ~30 seconds.

---

That's it. WordPress rollbacks won't touch this ever again.
