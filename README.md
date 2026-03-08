# OrderTrack

Garment order and lab test management app. Single-file HTML — runs entirely in the browser, auth powered by Supabase.

---

## 🚀 Deploy to Vercel

### Step 1 — Push to GitHub
1. Create a new repo on [github.com](https://github.com)
2. Upload the two files (`index.html` + `vercel.json`) to the repo
3. Or use GitHub Desktop / git CLI:
```bash
git init
git add .
git commit -m "Initial deploy"
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### Step 2 — Deploy on Vercel
1. Go to [vercel.com](https://vercel.com) → **Add New Project**
2. Import your GitHub repo
3. Leave all settings as default — Vercel auto-detects the static site
4. Click **Deploy**
5. Your app is live at `https://your-project.vercel.app`

---

## 🔐 Supabase Auth Setup

Your Supabase project: `https://oiycwxqymcuaaxqpmuch.supabase.co`

### Add the Vercel URL to Supabase allowed redirects
1. Go to Supabase → **Authentication → URL Configuration**
2. Under **Site URL** — set it to your Vercel URL (e.g. `https://ordertrack.vercel.app`)
3. Under **Redirect URLs** — add your Vercel URL

### Create users
1. Go to Supabase → **Authentication → Users**
2. Click **Add user → Create new user**
3. Enter email + password → **Create**
4. The user signs in, goes to **Account → Display Name** to set a username

---

## 👤 Username Login

After a user signs in once with their email, they can set a display name in **Account Settings**. From that point on they can log in using either their email or their display name as a username.

---

## 📦 Files

| File | Description |
|------|-------------|
| `index.html` | The full app (HTML + CSS + JS, single file) |
| `vercel.json` | Vercel routing + security headers config |

---

## 🛠 Tech Stack

- Pure HTML / CSS / JS — no build step needed
- [Supabase](https://supabase.com) — authentication
- [Flatpickr](https://flatpickr.js.org) — date pickers
- [SheetJS](https://sheetjs.com) — Excel export
- [Google Fonts](https://fonts.google.com) — Outfit + Space Mono
