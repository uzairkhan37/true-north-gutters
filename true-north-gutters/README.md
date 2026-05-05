# True North Gutters — Website

Marketing site for **True North Gutters**. Plain HTML, CSS, and JavaScript — no build step, no frameworks. Deploys to Vercel in one click.

## What's in here

```
true-north-gutters/
├─ index.html      ← the website page
├─ styles.css      ← all styling (navy + steel + white)
├─ script.js       ← scroll animations, mobile menu, FAQ
├─ logo.svg        ← built-in logo (used until you swap in your real one)
├─ logo.png        ← (optional — drop your real logo here)
├─ vercel.json     ← Vercel config
├─ .gitignore
├─ README.md       ← this file
└─ DEPLOY.md       ← step-by-step GitHub + Vercel guide
```

## The basics

- **Phone:** 226-507-0981 — wired into every "Call" button as `tel:` so phones dial it.
- **Email:** truenorthgutterservice@gmail.com — wired as `mailto:` so the visitor's email app opens pre-filled.
- **Logo:** the site shows `logo.svg` by default. Drop a `logo.png` in this folder and it will use that automatically.

## To preview the site on your computer

Just double-click `index.html`. It opens in your browser. No server needed.

## To deploy it to the internet

Read **DEPLOY.md** — it walks you through GitHub and Vercel start to finish.

## To change something later

| You want to change… | Open this file | Look for… |
|---|---|---|
| Phone number | `index.html` | `226-507-0981` (also `+12265070981` in `tel:` links) |
| Email address | `index.html` | `truenorthgutterservice@gmail.com` |
| Headline / hero copy | `index.html` | `<h1 class="hero__title">` |
| Services or descriptions | `index.html` | the `<section class="services">` block |
| Colors | `styles.css` | the `:root` block at the top — change `--navy`, `--steel`, etc. |
| FAQ questions | `index.html` | the `<section class="faq">` block |
