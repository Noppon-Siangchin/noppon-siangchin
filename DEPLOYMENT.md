# Deployment Guide

This guide walks through deploying the landing page to GitHub Pages.

**Estimated time:** 10–15 minutes (including first-time GitHub setup if needed)

---

## Prerequisites

- A GitHub account (free) — sign up at https://github.com/join
- Git installed on your machine — check with `git --version`
- This folder downloaded to your local machine

---

## Method 1: Using Claude Code (Recommended)

If you have Claude Code installed, just open this folder and ask Claude:

```
Please follow the instructions in CLAUDE.md and DEPLOYMENT.md to deploy this site to GitHub Pages.
My GitHub username is: [your-username]
My preferred repo name is: [repo-name]
```

Claude Code will handle the rest.

---

## Method 2: Manual Deployment

### Step 1: Create a GitHub Repository

1. Go to https://github.com/new
2. **Repository name:** `noppon-siangchin` (or your preferred name)
3. **Description:** "Personal digital business card and landing page"
4. **Visibility:** Public (required for free GitHub Pages)
5. **Initialize repository:** Leave UNCHECKED (we have files already)
6. Click **Create repository**

### Step 2: Initialize Git Locally

Open a terminal in this folder and run:

```bash
# Initialize git repo
git init

# Configure git (if not done already)
git config user.name "Noppon Siangchin"
git config user.email "noppon@senestia.com"

# Add all files
git add .

# Create first commit
git commit -m "Initial commit: digital business card landing page"

# Rename branch to main
git branch -M main
```

### Step 3: Connect to GitHub and Push

Replace `[username]` and `[repo-name]` with your actual values:

```bash
# Add GitHub as remote
git remote add origin https://github.com/[username]/[repo-name].git

# Push to GitHub
git push -u origin main
```

If prompted for credentials:
- Username: your GitHub username
- Password: use a **Personal Access Token** (not your GitHub password)
  - Create one at: https://github.com/settings/tokens
  - Scope needed: `repo`

### Step 4: Enable GitHub Pages

1. Go to your repo on GitHub: `https://github.com/[username]/[repo-name]`
2. Click **Settings** (top tab)
3. Scroll to **Pages** in the left sidebar
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 2–5 minutes for first deployment

### Step 5: Verify Deployment

1. Refresh the Settings → Pages page
2. You should see: **"Your site is live at https://[username].github.io/[repo-name]/"**
3. Click the link to verify the site loads
4. Test on mobile by scanning a QR code that points to this URL

---

## Step 6 (Optional): Custom Domain

If you've purchased a custom domain (e.g., `noppon.dev`):

### A. Configure DNS

In your domain registrar's DNS settings, add these records:

**For apex domain (noppon.dev):**
```
Type    Name    Value
A       @       185.199.108.153
A       @       185.199.109.153
A       @       185.199.110.153
A       @       185.199.111.153
```

**For subdomain (www.noppon.dev):**
```
Type    Name    Value
CNAME   www     [username].github.io
```

### B. Add Custom Domain to GitHub

1. Go to Settings → Pages
2. Under **Custom domain**, enter: `noppon.dev`
3. Click **Save**
4. Wait for DNS check (can take 24 hours, usually faster)
5. Enable **Enforce HTTPS** once available

### C. Add CNAME File

Create a file in this repo named `CNAME` (no extension) with your domain:

```
noppon.dev
```

Commit and push it:

```bash
echo "noppon.dev" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```

---

## Updating the Site

After making changes locally:

```bash
git add .
git commit -m "Update [what you changed]"
git push
```

GitHub Pages will auto-deploy within 1–2 minutes.

---

## Common Issues

### "Permission denied (publickey)"
You need to set up SSH keys, or use HTTPS instead:
```bash
git remote set-url origin https://github.com/[username]/[repo-name].git
```

### Site not loading after 5 minutes
- Check Settings → Pages → make sure status shows "Your site is live"
- Check Actions tab for failed deployments
- Try a hard refresh (Ctrl+Shift+R / Cmd+Shift+R)

### Images not displaying
- File names are case-sensitive: `business-card.png` ≠ `Business-Card.PNG`
- Check that files were actually pushed: `git ls-files`

### vCard download not working on iPhone
- This is normal for older iOS versions
- iOS 14+ should work; older versions may show the vCard as text
- Recommend the user save the LinkedIn URL instead as backup

---

## Quick Reference

| Action | Command |
|---|---|
| First-time setup | `git init && git add . && git commit -m "Initial commit"` |
| Connect to GitHub | `git remote add origin https://github.com/USER/REPO.git` |
| Push changes | `git push` |
| Pull latest | `git pull` |
| Check status | `git status` |
| View history | `git log --oneline` |

---

## Need Help?

- **GitHub Docs on Pages:** https://docs.github.com/en/pages
- **DNS not working:** Wait up to 24 hours, then check with `dig noppon.dev`
- **HTTPS not enforcing:** Wait 24 hours after adding custom domain
