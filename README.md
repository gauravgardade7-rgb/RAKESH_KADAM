# RK Auto Garage — Website

A ready-to-edit website for RK Auto Garage (Rakesh Kadam). Built with plain HTML/CSS/JS — no build tools needed, just open it in VS Code.

## 1. Open in VS Code

1. Unzip/copy this folder anywhere on your computer.
2. Open VS Code → File → Open Folder → select `rk-auto-garage`.
3. Install the **"Live Server"** extension in VS Code (Extensions tab → search "Live Server").
4. Right-click `index.html` → **Open with Live Server**. The site opens in your browser and refreshes automatically as you edit.

## 2. Files

```
rk-auto-garage/
├── index.html      → all page content (text, sections)
├── css/style.css   → all colors, fonts, spacing
├── js/script.js    → mobile menu + contact form behavior
├── images/         → put your real photos here
└── README.md
```

## 3. Things to replace before you publish

Search `index.html` for these and swap in your real details:

| Find | Replace with |
|---|---|
| `+91XXXXXXXXXX` | Your real phone number (appears in Call buttons, WhatsApp links, and the schema block at the top) |
| `Your Shop No., Street Name, Area, City — PIN` | Your real address |
| `Mon – Sat, 9:00 AM – 8:00 PM` | Your real hours |
| Placeholder photo boxes (`.ph` / "Photo 1" etc.) | Real `<img src="images/your-photo.jpg">` tags |
| Service list, parts list | Add/remove to match what you actually offer |

## 4. Adding real photos

Put image files in the `images/` folder, then replace a placeholder block like:

```html
<div class="gallery-item ph">Photo 1<br><small>e.g. custom exhaust build</small></div>
```

with:

```html
<div class="gallery-item">
  <img src="images/custom-exhaust.jpg" alt="Custom exhaust build">
</div>
```

## 5. Getting the contact form to actually send you messages

Right now the form just shows a thank-you message on screen — it doesn't email or message anyone yet, since a plain HTML file can't send messages by itself. Easiest free options:
- **Formspree** (formspree.io) — add their form endpoint as the form's `action`, no backend needed.
- **Google Forms** — embed a Google Form instead, responses land in a spreadsheet automatically.

## 6. Showing up on Google Search

Building the site doesn't automatically put it on Google — three steps get you there:

1. **Host it somewhere public.** Free/easy options: GitHub Pages, Netlify, or Vercel. Or buy hosting + a domain (e.g. `rkautogarage.com`) from providers like Hostinger or GoDaddy.
2. **Submit it to Google Search Console** (search.google.com/search-console) — add your site, verify ownership, and submit it for indexing. This is usually what gets a new site showing up in search within days rather than weeks.
3. **Set up a free Google Business Profile** (google.com/business) — this is actually the biggest lever for a local garage. It's what makes you show up on Google Maps and in the local "3-pack" when people search "bike garage near me" — much more effective for foot traffic than the website ranking alone.

Once hosted, also update these two lines in `index.html` to your real domain:
```html
<link rel="canonical" href="https://www.rkautogarage.com/">
<meta property="og:url" content="https://www.rkautogarage.com/">
```
