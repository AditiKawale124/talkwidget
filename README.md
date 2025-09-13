# TalkWidget for Nextcloud Dashboard

TalkWidget is a custom Nextcloud Dashboard widget that integrates with **Nextcloud Talk** and displays recent room messages directly on the Dashboard.  
This project uses **PHP (Nextcloud App Framework)** and **Webpack (JS/React/Vue frontend)**.

---

## 🚀 Features
- Custom Dashboard widget named **Talk Widget**
- Compiled frontend bundle with Webpack
- Integration point for fetching Talk API messages
- Easy to extend with Vue/React components

---

## 📂 Project Structure
```
apps/talkwidget/
├── appinfo/
│   └── info.xml
├── js/
│   └── talkwidget.js
├── lib/
│   └── Dashboard/
│       └── TalkWidget.php
├── templates/
│   └── main.php
├── package.json
├── webpack.config.js
└── README.md
```

---

## ⚙️ Setup Instructions

### 1. Clone into Nextcloud apps folder
```bash
cd /var/www/html/apps
git clone <repo-url> talkwidget
cd talkwidget
```

### 2. Install dependencies
```bash
npm install
```

### 3. Build frontend assets
For **production**:
```bash
npx webpack --mode production
```

For **development with auto-watch**:
```bash
npx webpack --mode development --watch
```

### 4. Enable app in Nextcloud
```bash
php occ app:disable talkwidget
php occ app:enable talkwidget
```

### 5. Check Dashboard
Go to **Nextcloud Dashboard**, and you should see the new **Talk Widget**.

---

## 🛠 Development Notes
- Frontend entry: `js/talkwidget.js`  
- Bundled file: `talkwidget.bundle.js` (auto-compiled into `js/`)  
- Template: `templates/main.php` (mount point for JS app)  
- Backend: `lib/Dashboard/TalkWidget.php` (implements `IDashboardWidget`)  

---

## 📌 Roadmap
- [ ] Display Talk rooms
- [ ] Show latest messages
- [ ] Add reply / react buttons
- [ ] User settings for room selection

---

## 🧑‍💻 Contributors
- Mayuri Mahajan
- Yashika Chawla
-Aditi Kawale
---

## 📜 License
MIT or AGPL-3.0 (depending on your Nextcloud app distribution needs)
