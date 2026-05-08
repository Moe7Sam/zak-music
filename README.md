# 🎸 Zak Electronics & Music — Landing Page

A modern, premium single-page website for **Zak Electronics and Music**, Al Karamah, Dubai.  
Built as a static HTML file — no frameworks, no build tools, no server required.

**Live Demo:** `https://YOUR-USERNAME.github.io/zak-music/`

---

## 📋 What's on the Page

| # | Section | Description |
|---|---------|-------------|
| 1 | **Hero** | Full-screen cinematic intro with animated notes and scroll indicator |
| 2 | **Instruments** | Featured instrument grid with hover effects and pricing |
| 3 | **Beginner Packages** | Guitar, Keyboard & Ukulele starter kits with WhatsApp enquiry buttons |
| 4 | **About** | Store story, quote, and animated stats counter |
| 5 | **Google Reviews** | 6 customer review cards with star ratings |
| 6 | **WhatsApp CTA** | Direct chat call-to-action section |
| 7 | **Video / Reel** | YouTube reel embed (click-to-load) |
| 8 | **Location & Contact** | Map placeholder, address, phone, hours, email |
| 9 | **Instagram & TikTok** | Social grid with follow buttons |
| 10 | **Footer** | Links, tagline, copyright |

---

## 🚀 Deploy on GitHub Pages (5 Minutes)

### Step 1 — Create a GitHub Repository

1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Click the **+** button → **New repository**
3. Name it: `zak-music` (or anything you like)
4. Set visibility to **Public**
5. Click **Create repository**

### Step 2 — Upload the Files

**Option A — Drag & Drop (easiest):**
1. On your new repo page, click **uploading an existing file**
2. Drag `index.html` and `README.md` into the upload area
3. Optionally add a `favicon.png` (see Favicon section below)
4. Click **Commit changes**

**Option B — Git (for developers):**
```bash
git clone https://github.com/YOUR-USERNAME/zak-music.git
cd zak-music
# Copy index.html and README.md into this folder
git add .
git commit -m "Initial launch"
git push origin main
```

### Step 3 — Enable GitHub Pages

1. Go to your repository → **Settings** tab
2. Scroll to **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Choose branch: `main` · folder: `/ (root)`
5. Click **Save**

### Step 4 — Your Site is Live

GitHub will show a banner:  
> ✅ Your site is published at `https://YOUR-USERNAME.github.io/zak-music/`

It usually takes **1–3 minutes** to go live. Refresh the Settings → Pages tab to see the URL.

---

## ✏️ How to Edit the Site

All editable content is inside `index.html`. Open it in any text editor  
(Notepad, VS Code, Sublime, etc.) and look for the `✏️` comment markers.

---

### 📱 Change the WhatsApp Number

Search the file for `971XXXXXXXXX` — replace **all occurrences** with the real number.

**Format:** country code + number, no spaces, no dashes, no `+`  
**UAE example:** `971501234567` means `+971 50 123 4567`

There are **10 places** to update. Use Find & Replace (`Ctrl+H` / `Cmd+H`):
- Find: `971XXXXXXXXX`
- Replace: `971501234567` ← your real number

---

### 💰 Change Prices

Search for these lines and edit the number:

```html
<!-- Guitar Starter -->
<div class="package-price">AED 299 <small>/ complete set</small></div>

<!-- Keyboard Bundle -->
<div class="package-price">AED 549 <small>/ complete set</small></div>

<!-- Ukulele Kit -->
<div class="package-price">AED 149 <small>/ complete set</small></div>
```

Instrument prices appear inside `.instrument-price` divs:
```html
<div class="instrument-price">From AED 199 · All Brands</div>
```

---

### 📦 Edit Package Features

Each package has a `<ul class="package-features">` list.  
Add, remove, or change `<li>` items freely:

```html
<ul class="package-features">
  <li>Acoustic guitar (full-size or 3/4)</li>
  <li>Picks, tuner &amp; spare strings</li>
  <li>Carrying bag included</li>
  <!-- Add more items here -->
</ul>
```

---

### 📍 Update Address & Contact

Find the Location section (search for `id="location"`) and edit:

```html
<!-- Address -->
Zak Electronics &amp; Music<br>
Al Karamah, Abu Dhabi Road<br>
Dubai, United Arab Emirates

<!-- Phone -->
<a href="tel:+971XXXXXXXXX">+971 XX XXX XXXX</a>

<!-- Email -->
<a href="mailto:info@zakmusic.ae">info@zakmusic.ae</a>

<!-- Opening hours -->
<div class="hours-row"><span>Sat – Thu</span><span>10am – 9pm</span></div>
<div class="hours-row"><span>Friday</span><span>2pm – 9pm</span></div>
```

**Google Maps link:** Search the store on Google Maps → Share → Copy link.  
Paste the URL into:
```html
<a href="YOUR_GOOGLE_MAPS_LINK" class="map-open-btn" ...>Open in Maps</a>
```

---

### 🎬 Change the YouTube Video

In the `<script>` section at the bottom, find:
```javascript
src="https://www.youtube.com/embed/dQw4w9WgXcQ?autoplay=1"
```
Replace `dQw4w9WgXcQ` with your YouTube video ID.  
The video ID is the 11-character code in any YouTube URL:  
`https://youtube.com/watch?v=` **`XXXXXXXXXXX`**

---

### 📸 Update Social Media Links

Find the Social section (search for `id="social"`) and update:

```html
<!-- Instagram button -->
<a href="https://www.instagram.com/YOUR_HANDLE" ...>
  <span>📸</span> @YourHandle
</a>

<!-- TikTok button -->
<a href="https://www.tiktok.com/@YOUR_HANDLE" ...>
  <span>🎵</span> @YourHandle
</a>
```

---

### 🔍 Update SEO Tags

At the top of the file, update:

```html
<!-- Your live GitHub Pages URL -->
<link rel="canonical" href="https://YOUR-USERNAME.github.io/zak-music/">

<!-- Open Graph image (shown when shared on WhatsApp/Facebook) -->
<meta property="og:image" content="https://YOUR-USERNAME.github.io/zak-music/og-image.jpg">
```

**Recommended OG image size:** 1200 × 630px — upload it to your repo as `og-image.jpg`.

---

### 🎨 Add a Favicon

1. Create or download a small square icon (ideally 512×512px PNG)
2. Save it as `favicon.png` in the same folder as `index.html`
3. Upload it to GitHub alongside `index.html`

The `<head>` already references it:
```html
<link rel="icon" type="image/png" href="favicon.png">
```

Free favicon generators: [favicon.io](https://favicon.io) · [realfavicongenerator.net](https://realfavicongenerator.net)

---

## 📁 File Structure

```
zak-music/
├── index.html      ← The entire website (edit this)
├── README.md       ← This guide
├── favicon.png     ← Your store icon (add this)
└── og-image.jpg    ← Social share image (add this, 1200×630px)
```

---

## 🛠️ No-Code Editing Tools

If you prefer a visual editor over raw HTML:

- **[VS Code](https://code.visualstudio.com/)** — Free, desktop, best experience
- **[Notepad++](https://notepad-plus-plus.org/)** — Lightweight Windows editor
- **[github.dev](https://github.dev)** — Press `.` on your repo to open VS Code in the browser, no install needed

---

## ✅ Pre-Launch Checklist

- [ ] WhatsApp number updated (all 10 occurrences)
- [ ] Phone number updated in contact section and footer
- [ ] Email address updated (`info@zakmusic.ae` → real email)
- [ ] Google Maps link updated with real store location
- [ ] YouTube video ID replaced with real reel
- [ ] Instagram handle updated
- [ ] TikTok handle updated
- [ ] `<link rel="canonical">` URL updated with real GitHub Pages URL
- [ ] `og:image` and `og:url` updated
- [ ] `favicon.png` uploaded
- [ ] `og-image.jpg` uploaded (1200×630px)
- [ ] GitHub Pages enabled in repository Settings → Pages
- [ ] Tested on mobile

---

## 📞 Support

Questions about this demo? Want changes to the design, extra sections, or a custom domain?  
Get in touch through WhatsApp or your preferred channel.

---

*Built with pure HTML, CSS & vanilla JS — no dependencies, no frameworks, no hosting costs.*
