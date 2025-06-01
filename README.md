# 🚀 How to Install Nativefier on Arch Linux with i3 WM 🖥️✨

---

## 1️⃣ Install Node.js & npm

Nativefier needs Node.js (v12+) and npm. Run:

```bash
sudo pacman -Syu nodejs npm
```

⚡️ Make sure your system is updated first!

---

## 2️⃣ Install Nativefier globally

```bash
sudo npm install -g nativefier
```

✅ This installs Nativefier so you can run it anywhere.

---

## 3️⃣ Verify installation

```bash
nativefier --version
```

🔍 You should see the version number printed.

---

## 4️⃣ Create your first desktop app 📦

Example: Wrap Gmail as a desktop app

```bash
nativefier "https://mail.google.com"
```

✨ This creates a folder with your app in the current directory.

---

## 5️⃣ Run Nativefier apps on i3 🪟

* The app executable is inside the generated folder, e.g.:

```bash
./mail-linux-x64/mail
```

* To launch quickly, add an i3 keybinding in your config (`~/.config/i3/config`):

```config
bindsym $mod+g exec ~/path/to/mail-linux-x64/mail
```

Reload i3 config with `$mod+Shift+r` 🔄

---

## 💡 Tips for i3 users

* Nativefier apps behave like normal windows — tile, float, or fullscreen 🪟
* Manage web apps on separate workspaces for focus 🎯
* Rename or move apps anywhere for convenience 🚀
