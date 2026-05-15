# Instructions for Claude Code

This file gives you context about this project and what needs to be done.

## Project Context

This is a personal digital business card landing page for **Noppon "Sun" Siangchin**, Senior Data Analyst at Senestia Company Limited. The site is built as static HTML/CSS/JS and is intended to be deployed to **GitHub Pages**.

## Owner / User

- **Name:** Noppon Siangchin (Sun)
- **Role:** Senior Data Analyst at Senestia
- **GitHub Username:** [TO BE FILLED IN BY USER — ask if not known]
- **Located:** Colchester, UK
- **Language preference:** Thai or English (user is bilingual; Thai preferred for casual conversation)

## Project Goal

Deploy `index.html` to GitHub Pages so it's publicly accessible at:
- `https://[username].github.io/[repo-name]/`
- or a custom domain in the future

The deployed URL will be encoded into a QR code on physical business cards.

## What You Need to Do

Follow the steps in `DEPLOYMENT.md`. In summary:

1. **Initialize a Git repository** in this directory
2. **Help the user create a GitHub repository** (or use their existing one)
3. **Push the code** to GitHub
4. **Enable GitHub Pages** for the repository (Settings → Pages → Source: main branch)
5. **Verify the site is live** at the GitHub Pages URL
6. **Provide the user with the final URL** so they can use it for the QR code

## Important Notes

### Do NOT change without asking:
- The visual design of `index.html` (colors, fonts, layout)
- The `business-card.png` image
- Contact information in the vCard generator function

### You CAN update:
- The `og:image` URL and other meta tags if needed for full URL (e.g., `https://username.github.io/repo/business-card.png` instead of relative path)
- The footer year if outdated
- Any typos or broken links
- The README placeholder URL (`[your-github-username]/[repo-name]`) with actual values

### Style preferences:
- The user values clean, professional design
- Editorial/refined aesthetic — NOT generic AI-style
- Sub-bullets, em dashes, and elegant typography are part of the look

## Repository Setup Recommendations

**Repo name suggestions** (in order of preference):
1. `noppon-siangchin` — clean, professional, uses real name
2. `sun-card` — short, memorable
3. `digital-card` — generic but functional

**Repo visibility:** Public (required for free GitHub Pages)

**Branch:** `main`

**Description:** "Personal digital business card and landing page — Noppon Siangchin, Senior Data Analyst at Senestia"

## After Deployment

Once the site is live, remind the user to:

1. **Test the URL** on both iPhone and Android
2. **Generate the QR code** using the `qr-generator.html` tool with the new URL
3. **Update social profiles** (LinkedIn) with the new URL
4. **Optional:** Consider purchasing a custom domain (e.g., `noppon.dev`) for £10-15/year for a more professional URL

## Verification Checklist

After deployment, verify:

- [ ] Site loads at `https://[username].github.io/[repo-name]/`
- [ ] HTTPS works (green padlock)
- [ ] Business card image displays correctly
- [ ] "Save Contact" button downloads a working .vcf file
- [ ] All contact links work (phone numbers, email, LinkedIn)
- [ ] Site is responsive on mobile (test on real device or DevTools)
- [ ] Page loads in under 2 seconds
- [ ] Meta tags work correctly (test by sharing the URL on LinkedIn/Slack to see preview)

## Troubleshooting

**If GitHub Pages doesn't deploy:**
- Wait 2-5 minutes after enabling Pages — first deploy is slow
- Check Settings → Pages → make sure Source is set to `main` branch, `/ (root)` folder
- Check Actions tab for any deployment errors

**If images don't load:**
- File names are case-sensitive on GitHub Pages
- Make sure `business-card.png` exists in the root (not in a subfolder)

**If "Save Contact" doesn't work:**
- This requires JavaScript — make sure the user isn't blocking JS
- The function downloads a Blob — works on all modern browsers
