# 🧶 Crochetelo Website – Complete Beginner's Guide
## Build, Run & Host Your Website Step by Step

---

## 📁 YOUR FILES (already created for you)
```
crochetelo-website/
  ├── index.html   ← Homepage
  ├── shop.html    ← Shop page
  ├── style.css    ← All styles/design
  └── script.js   ← Interactivity
```

---

## STEP 1 – Install VS Code (Code Editor)

1. Go to **https://code.visualstudio.com**
2. Click **Download for Windows** (or Mac/Linux)
3. Run the installer and click **Next** through all steps
4. Launch VS Code

---

## STEP 2 – Open Your Project in VS Code

1. Open VS Code
2. Click **File → Open Folder**
3. Select the folder **crochetelo-website** (the one you downloaded)
4. You'll see all 4 files on the left panel

---

## STEP 3 – Install Live Server Extension (see your website live)

1. In VS Code, click the **Extensions icon** on the left (looks like 4 squares)
2. Search: **Live Server**
3. Click **Install** on the one by Ritwick Dey
4. After installing, right-click on **index.html** in the file panel
5. Click **"Open with Live Server"**
6. Your browser will open with your website at `http://127.0.0.1:5500`
7. **Every time you save a file, the browser refreshes automatically!**

---

## STEP 4 – Customize Your Website

### Change the Brand Name
Open `index.html` and find:
```html
<span class="logo-text">Crochetelo
```
Replace `Crochetelo` with your own brand name.

### Change Colors
Open `style.css` and find the `:root` section at the top:
```css
:root {
  --dark:   #1a1209;    ← Very dark brown (navbar, footer)
  --brown:  #3b1f0a;    ← Logo color
  --gold:   #b07d3a;    ← Highlight color
  --accent: #c0392b;    ← Red accent (used for icons)
  --light:  #faf6f0;    ← Page background
}
```
Change the `#hex` values to any color you want.
Use this tool to pick colors: **https://colorpicker.me**

### Change Product Names & Prices
In `index.html`, find each product card:
```html
<h3>Checkered Kimono</h3>
<p class="price">₦ 305,000</p>
```
Change the name and price to match your real products.

### Add Your Own Photos
1. Put your product images inside the `crochetelo-website` folder
2. Name them simply, e.g. `dress1.jpg`, `kimono.jpg`
3. In index.html, find:
```html
<img src="https://images.unsplash.com/..." alt="Checkered Kimono"/>
```
Replace the URL with your image filename:
```html
<img src="dress1.jpg" alt="Checkered Kimono"/>
```

### Add More Products
Copy and paste this block inside the `<div class="products-grid">`:
```html
<div class="product-card" data-category="women">
  <div class="product-img-wrap">
    <img src="your-image.jpg" alt="Product Name"/>
    <button class="wishlist-btn">♡</button>
  </div>
  <h3>Your Product Name</h3>
  <p class="product-subtitle">Short description here</p>
  <p class="price">₦ 200,000</p>
</div>
```
Change `data-category` to: `women`, `men`, or `unisex`

---

## STEP 5 – Host Your Website for FREE (Go Live!)

### Option A: Netlify (EASIEST – Recommended for beginners)

1. Go to **https://netlify.com** and sign up (free)
2. Click **"Add new site" → "Deploy manually"**
3. **Drag and drop** your entire `crochetelo-website` folder onto the page
4. Wait 30 seconds – Netlify gives you a live URL like:
   `https://amazing-site-123.netlify.app`
5. To update: just drag-drop your folder again

**Custom domain (optional):**
- Go to **Site settings → Domain management → Add custom domain**
- Buy a domain at **Namecheap.com** (~$10/year) e.g. `crochetelo.com`
- Follow Netlify's instructions to link it

---

### Option B: GitHub Pages (also free)

1. Install **Git**: https://git-scm.com/downloads
2. Create a free account at **https://github.com**
3. Click **New repository**, name it `crochetelo-website`, make it **Public**
4. In VS Code, open the Terminal (View → Terminal) and type:
```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/crochetelo-website.git
git push -u origin main
```
5. On GitHub: go to **Settings → Pages → Source → main branch → Save**
6. Your site is live at: `https://YOUR-USERNAME.github.io/crochetelo-website`

---

## STEP 6 – What to Download (Summary)

| Tool | What For | Link |
|------|----------|------|
| **VS Code** | Writing code | https://code.visualstudio.com |
| **Live Server** (VS Code Extension) | Preview website | Search in VS Code Extensions |
| **Git** (optional) | Upload to GitHub | https://git-scm.com |
| **Node.js** (later, when you grow) | Advanced features | https://nodejs.org |

---

## TIPS FOR MAKING IT LOOK MORE LIKE CROCHETELO

1. **Use your own real photos** – the biggest upgrade you can make
2. **Keep prices in ₦** – already set up in the code
3. **Add WhatsApp link** – replace a social icon with:
   ```html
   <a href="https://wa.me/2348012345678">WhatsApp</a>
   ```
4. **Add more pages** – copy `shop.html` and rename it `contact.html` for a contact page

---

## NEED HELP?
- Google: "HTML CSS tutorial for beginners" 
- YouTube: **The Odin Project** or **freeCodeCamp**
- Free full course: **https://www.freecodecamp.org**

Happy building! 🧶✨
