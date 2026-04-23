# 🏛️ TROY Perfumes — Website

> A luxury perfume storefront with an animated shutter entrance, live weather effects, and a full admin control panel.

---

## 📁 Project Structure

```
troy-website/
├── index.html          ← Main storefront (customer-facing)
├── admin/
│   └── index.html      ← Admin control panel (password protected)
├── assets/             ← Place images / icons here
├── 404.html            ← Custom "Page Not Found" page
├── robots.txt          ← SEO crawler instructions
├── sitemap.xml         ← SEO sitemap
├── manifest.json       ← PWA / mobile app manifest
├── CNAME               ← Custom domain (edit before deploying)
└── README.md           ← This file
```

---

## 🚀 Deploy to GitHub Pages

1. Push this folder to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to **`main` branch / `/ (root)`**
4. Your site will be live at `https://<your-username>.github.io/<repo-name>/`

### Using a Custom Domain
1. Edit `CNAME` and replace the placeholder with your domain (e.g. `troyperfumes.com`)
2. In your DNS provider, add an **A record** pointing to GitHub Pages IPs:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
3. Or add a **CNAME record** pointing `www` → `<your-username>.github.io`

---

## 🌐 Deploy to Any Web Host (cPanel / FTP)

1. Upload all files to your `public_html` folder
2. Make sure `index.html` is at the root
3. Access admin panel at `yourdomain.com/admin/`

---

## 🔐 Admin Panel

Access the admin panel at `/admin/` or `/admin/index.html`.

Default credentials are managed inside `admin/index.html` — search for `ADMIN_PASS` to change the password before going live.

---

## ✨ Features

- 🏪 Animated storefront shutter entrance
- 🌦️ Live weather detection & animated effects (rain, snow, thunder, clear sky)
- 🕐 Real-time clock display on shutter
- 🛍️ Full product catalogue with cart system
- 🎨 Admin panel: product management, orders, customers, analytics
- 📱 Mobile responsive

---

## 📝 Notes

- All CSS and JavaScript are **self-contained** inside the HTML files — no build step needed
- External dependencies (Google Fonts, Font Awesome) are loaded from CDN
- Weather data is fetched from [Open-Meteo](https://open-meteo.com/) (free, no API key required)
- Geolocation uses browser API with IP fallback via [ipapi.co](https://ipapi.co/)
