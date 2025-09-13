# TalkWidget: Nextcloud Chat Dashboard

TalkWidget is a custom widget for the **Nextcloud Dashboard** that integrates with **Nextcloud Talk** and displays recent messages from chat rooms directly on the Dashboard. This enhances collaboration by providing quick access to important messages without switching between apps.

---

## 🚀 Features
- Custom Dashboard widget named **Talk Widget**.
- Fetches and displays messages from Nextcloud Talk API.
- Easy to extend with React or Vue components.
- Supports production and development builds with Webpack.
- Simple setup using Nextcloud’s app framework.

---

## 📂 Project Structure
apps/talkwidget/
├── appinfo/
│ └── info.xml
├── js/
│ └── talkwidget.js
├── lib/
│ └── Dashboard/
│ └── TalkWidget.php
├── templates/
│ └── main.php
├── package.json
├── webpack.config.js
└── README.md


---

## 📦 Technologies Used
- **Backend:** PHP (Nextcloud App Framework)
- **Frontend:** JavaScript, React/Vue, Webpack
- **APIs:** Nextcloud Talk API
- **Build tools:** npm, Webpack

---

## ⚙️ Setup Instructions

1. **Clone into Nextcloud apps folder**
    ```bash
    cd /var/www/html/apps
    git clone https://github.com/yourusername/talkwidget.git
    cd talkwidget
    ```

2. **Install dependencies**
    ```bash
    npm install
    ```

3. **Build frontend assets**
    - For **production**:
      ```bash
      npx webpack --mode production
      ```
    - For **development with auto-watch**:
      ```bash
      npx webpack --mode development --watch
      ```

4. **Enable the app in Nextcloud**
    ```bash
    php occ app:disable talkwidget
    php occ app:enable talkwidget
    ```

5. **Check the Dashboard**
   Visit the Nextcloud Dashboard to see the new **Talk Widget** in action.

---

## 📈 Roadmap
- Display list of Talk rooms.
- Show latest messages with timestamps.
- Add reply and reaction buttons.
- Allow users to select rooms and configure settings.

---

## 👥 Contributors
- Mayuri Mahajan
- Yashika Chawla
- Aditi Kawale

---

## 📜 License
This project is licensed under **MIT** or **AGPL-3.0**, depending on your distribution preferences.

---

## 📞 Contact
For questions or feedback, reach out to the contributors via the hackathon platform or open an issue in this repository.

---
