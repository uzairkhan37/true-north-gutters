# Deploying True North Gutters to the Internet

This is a beginner-friendly walkthrough. Read it top to bottom — every step matters but none of them are hard. Total time: about 20 minutes the first time, 30 seconds every time after that.

---

## What we're doing, in plain English

Right now your website lives in a folder on your computer. We're going to:

1. **Put your real logo in the folder** (optional but recommended)
2. **Push the folder to GitHub** — GitHub is like Google Drive for code. It stores your project online so other tools can read it.
3. **Connect GitHub to Vercel** — Vercel takes whatever's in your GitHub project and turns it into a live website at a real URL.
4. **Get your URL** — something like `true-north-gutters.vercel.app` (free), or your own domain like `truenorthgutters.ca` later if you want.

After this is set up, every time you change a file and push it to GitHub, Vercel automatically rebuilds your live website. You never touch a server.

---

## Step 0 — One-time setup (15 minutes)

You need three free accounts. If you already have any, skip those.

1. **GitHub account** → https://github.com/signup
2. **Vercel account** → https://vercel.com/signup — when it asks how to sign up, **choose "Continue with GitHub"**. This automatically links the two.
3. **GitHub Desktop** (the app, not the website) → https://desktop.github.com — this lets you push code without learning command-line stuff. Install it and sign in with the GitHub account you just made.

That's it. You're set up forever.

---

## Step 1 — Drop in your real logo (optional)

The site already has a built-in logo (`logo.svg`) so it works out of the box. If you'd rather use your real logo image:

1. Save your True North Gutters logo as a PNG file (transparent background works best).
2. Name the file exactly `logo.png` (lowercase, no spaces).
3. Drag that `logo.png` file **into the `true-north-gutters` folder** — same folder as `index.html`.

That's it. The website automatically prefers `logo.png` over the built-in SVG. If `logo.png` isn't there, it falls back to the SVG. Either way the site works.

> **Tip:** Open `index.html` in your browser by double-clicking it to confirm the logo looks right before you push anything online.

---

## Step 2 — Put your project on GitHub

1. Open **GitHub Desktop**.
2. Top menu → **File → Add Local Repository…**
3. Click **Choose…** and pick the `true-north-gutters` folder.
4. GitHub Desktop will say "*This directory does not appear to be a Git repository.*" Click the blue **"create a repository"** link in that message.
5. A dialog appears:
   - **Name:** `true-north-gutters` (or whatever you want — this becomes part of your URL)
   - **Description:** `True North Gutters website`
   - Leave the rest as default. Click **Create Repository**.
6. You'll see all your files listed on the left as "changes". In the bottom-left, type a **Summary** like `Initial website` and click **Commit to main**.
7. Now click the big **Publish repository** button at the top.
   - Uncheck **"Keep this code private"** if you want it public (recommended — it doesn't expose anything sensitive, and Vercel free tier needs public repos for easiest deployment).
   - Click **Publish Repository**.

Your project is now on GitHub. You can confirm by going to https://github.com → your profile → "Repositories".

---

## Step 3 — Deploy with Vercel

1. Go to https://vercel.com/new
2. You'll see a list of your GitHub repositories. Find **true-north-gutters** and click **Import**.
   - If you don't see it, click **"Adjust GitHub App Permissions"** and grant Vercel access to the repo.
3. Vercel will show a configuration screen. **You don't need to change anything.** It auto-detects this is a static site.
4. Click **Deploy**.
5. Wait ~30 seconds. You'll see fireworks (literally — Vercel celebrates).
6. Click **Continue to Dashboard**. Click **Visit** to open your live site.

Your URL will be something like:
- `https://true-north-gutters.vercel.app`
- or `https://true-north-gutters-uzairk.vercel.app`

**That's it. Your website is live on the internet.**

---

## Step 4 — Updating the site later

Whenever you change a file (edit text, swap the logo, tweak colors), here's the loop:

1. Make your change in the file (e.g. update the phone number in `index.html`).
2. Save the file.
3. Open **GitHub Desktop** — it will show your changes.
4. Bottom-left: type a Summary like `Update phone number` → click **Commit to main**.
5. Top: click **Push origin**.

Vercel sees the push automatically and redeploys your site within ~30 seconds. Refresh the live URL — your change is there.

You'll do this loop maybe 50 times in your life. It gets to be muscle memory in a week.

---

## Step 5 (optional, later) — Add a real domain

When you buy `truenorthgutters.ca` (or any other domain):

1. In Vercel → your project → **Settings → Domains**.
2. Type your domain → **Add**.
3. Vercel shows you 1-2 DNS records to add at your domain registrar (Namecheap, GoDaddy, etc.).
4. Add them. Wait 10-30 minutes. Done.

---

## Common hiccups

**"I don't see my files in the project after pushing."**
Make sure GitHub Desktop is pointed at the `true-north-gutters` folder, not its parent folder. The folder should contain `index.html` directly, not a subfolder containing it.

**"My logo doesn't show up after I dropped it in."**
Check the filename is exactly `logo.png` — all lowercase, no `Logo.PNG` or `logo (1).png`. Then refresh the page (Ctrl+Shift+R / Cmd+Shift+R for a hard refresh).

**"The page looks broken / unstyled."**
You probably uploaded `index.html` without `styles.css`. Make sure all four files (`index.html`, `styles.css`, `script.js`, `logo.svg`) are in the GitHub repo together.

**"I want to test before I push."**
Just double-click `index.html` on your computer. It opens in your browser exactly as it'll appear live. The only feature that won't work locally is the `tel:` link (most desktop browsers don't dial), but it works perfectly on phones.

---

## What to do next

After your first deployment, here are quick wins:

1. **Add real photos.** Take 4-6 photos of finished gutter work — before/afters are gold. We can add a gallery section.
2. **Add a real Google review badge** once you have a few reviews. The "★★★★★" placeholder in the trust bar is a stand-in.
3. **Put the URL on your truck, business cards, and Instagram bio.**

When you're ready for any of these, just ask — I'll walk you through it.
