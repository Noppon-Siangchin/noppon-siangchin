# Claude Code Prompts — Copy & Paste

Below are ready-to-use prompts for Claude Code. Copy whichever fits your situation, paste into Claude Code, and let it work.

---

## 🚀 Prompt 1: Full Deployment (Recommended)

**Use when:** You want Claude Code to do everything from start to finish.

**Before pasting:** Replace `[YOUR_GITHUB_USERNAME]` with your actual GitHub username.

```
Hi Claude. Please help me deploy this digital business card to GitHub Pages.

Context:
- My GitHub username is: [YOUR_GITHUB_USERNAME]
- I want the repo to be named: noppon-siangchin
- The site should be public
- All the files needed are in this folder

Please:
1. Read CLAUDE.md and DEPLOYMENT.md for full context
2. Check that Git is configured on my machine (if not, help me set it up)
3. Initialize a Git repository in this folder
4. Help me create the GitHub repo (you can guide me through the gh CLI or web UI)
5. Push all files to GitHub
6. Walk me through enabling GitHub Pages in the repo settings
7. Verify the site is live and give me the final URL

If you encounter any issues (auth, permissions, missing tools), stop and explain them clearly in Thai or English. I'm comfortable with the command line but not an expert.

After deployment, please:
- Update the README.md to replace [your-github-username]/[repo-name] placeholders with my actual values
- Test that the page loads correctly
- Give me a checklist of things to verify on my own
```

---

## ⚡ Prompt 2: I Already Have a Repo

**Use when:** You already created a GitHub repository and just need to push files.

```
Hi Claude. I have a GitHub repository already created at:
https://github.com/[username]/[repo-name]

Please:
1. Read CLAUDE.md for context
2. Initialize git in this folder
3. Push all files to the existing repo
4. Help me enable GitHub Pages in the settings (provide screenshots/guidance)
5. Give me the final live URL

If the repo already has files, ask me before overwriting anything.
```

---

## 🔧 Prompt 3: Custom Domain Setup

**Use when:** Your site is already deployed and you bought a custom domain.

```
Hi Claude. My site is live at https://[username].github.io/[repo-name]/

I just bought the domain: [your-domain.com]
I purchased it from: [Namecheap / Google Domains / Cloudflare / etc.]

Please help me:
1. Configure DNS records on my domain registrar
2. Add the CNAME file to my repo
3. Configure the custom domain in GitHub Pages settings
4. Enable HTTPS enforcement
5. Verify everything is working

Walk me through the DNS step carefully — I'm not sure where to find DNS settings on [registrar name].
```

---

## 🐛 Prompt 4: Troubleshooting

**Use when:** Something went wrong with deployment.

```
Hi Claude. I followed the deployment steps but [describe the problem here].

The error I see is:
[paste error message]

Please:
1. Read DEPLOYMENT.md and the Troubleshooting section
2. Help me diagnose the issue
3. Fix it step by step
4. Verify the fix worked
```

---

## 📝 Prompt 5: Update Content

**Use when:** You want to change something on the live site after initial deployment.

```
Hi Claude. My site is already deployed. I want to update [what you want to change].

For example:
- "Add a new section about my recent projects"
- "Change the tagline to: ..."
- "Update my LinkedIn URL to: ..."
- "Add a profile photo to the hero section"

Please make the change, then commit and push it. Confirm when the live site is updated.
```

---

## 💡 Tips for Working with Claude Code

### Before starting:
- Make sure you're in the project folder when you open Claude Code
- Have your GitHub username ready
- Have a Personal Access Token ready (if you don't use SSH keys)

### During the session:
- Read what Claude is about to do before approving destructive commands
- If Claude asks for permissions (e.g., `git push`), grant them
- Use Thai or English — Claude handles both fluently

### After deployment:
- **Save the final URL** somewhere safe (Notion, Notes app)
- **Bookmark the GitHub repo** for easy access
- **Test the URL on a real phone** before printing QR codes

---

## 📋 Pre-Flight Checklist

Before running any prompt above, make sure:

- [ ] You're in the project folder (`cd` to where these files live)
- [ ] Git is installed (`git --version` should work)
- [ ] You have a GitHub account
- [ ] You know your GitHub username
- [ ] You have a Personal Access Token OR SSH keys set up
- [ ] You have a stable internet connection

---

## 🎯 Recommended Workflow

1. **Open this folder** in your file explorer / VS Code
2. **Open Claude Code** in this folder
3. **Copy Prompt 1** (Full Deployment) from above
4. **Replace** `[YOUR_GITHUB_USERNAME]` with your real username
5. **Paste & send** to Claude Code
6. **Follow along** as Claude guides you
7. **Test the live URL** on your phone
8. **Update QR code** on `qr-generator.html` with the new URL
9. **Download QR PNG** and use it on your business cards / wallpaper / social profiles

---

Good luck, Sun! 🚀
