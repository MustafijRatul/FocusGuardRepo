# FocusGuard Pro 🛡️

**The ultimate productivity companion for Windows.**

FocusGuard Pro combines a powerful distraction blocker, a Pomodoro-style timer, and deep analytics into a stunning, modern interface featuring the Windows Acrylic (Glass) aesthetic.

![Version](https://img.shields.io/badge/version-11.6-blue) ![Python](https://img.shields.io/badge/python-3.10%2B-yellow) ![Platform](https://img.shields.io/badge/platform-Windows-0078D6)

---

## 🖼️ Screenshots

### **Dashboard**
*Track your current session, manage focus/break timers, and control ambient sounds.*
![Dashboard](screenshots/dashboard.png)

### **App Manager**
*Selectively block distracting applications with custom profiles.*
![App Blocking](screenshots/blocking.png)

### **Analytics**
*Visualize your productivity streaks and history over the last 7 days.*
![Analytics](screenshots/analytics.png)

---

## ✨ Key Features

### 🚀 **Productivity Engine**
*   **Smart Focus Timer:** A stunning circular timer supporting Focus and Break intervals.
*   **Task Intent:** Log exactly what you are working on before every session.
*   **Mini Mode:** A compact, always-on-top overlay to keep you aware of the time without cluttering your screen.

### 🚫 **Advanced App Blocking**
*   **Profile Management:** Create blocking profiles (e.g., "Deep Work", "Light Study") with specific app blocklists.
*   **Strict Mode:** Optionally force-kill distracting processes instead of just minimizing them.
*   **Smart Detection:** Automatically detects running windows and installed apps for easy selection.

### 📊 **Analytics & History**
*   **Interactive Charts:** View your focus performance over the last 7 days.
*   **Session Logs:** Detailed history of every session, including task names and duration.
*   **KPIs:** Track your daily focus time, streaks, and total distractions blocked.

### 🎨 **Modern UI/UX**
*   **Glass/Acrylic Effect:** Native Windows background blur integration.
*   **Theme Engine:** Switch between **Ambient** and **Dark** modes.
*   **Customization:** Choose from 6 neon accent colors and 3 button styles (Gradient, Solid, Glass).
*   **Responsive:** Optimized for High-DPI displays.

### 🎵 **Ambient Soundscapes**
*   Built-in audio engine playing Rain, Jungle, and Thunder sounds.
*   Support for uploading your own custom background music.

### 📅 **Scheduler**
*   Automate your day by scheduling specific blocking profiles to activate at specific times.

---

## 🛠️ Installation & Setup

### Prerequisites
*   Windows 10 or Windows 11 (Required for Glass effects).
*   Python 3.10 or higher.

### 1. Clone the Repository
```bash
git clone https://github.com/MustafijRatul/FocusGuardRepo.git
cd FocusGuardRepo
```

### 2. Install Dependencies
Create a virtual environment (recommended) and install the required libraries:

```bash
pip install PySide6 qtawesome pygetwindow pygame matplotlib
```

> **Note:** `winsound` is a standard Python library on Windows and does not need to be installed via pip.

### 3. Run the Application
```bash
python main.py
```

---

## 📦 Building an Executable

If you want to build a standalone `.exe` file to run without Python installed, use **PyInstaller**:

1. Install PyInstaller:
   ```bash
   pip install pyinstaller
   ```

2. Run the build command (ensure you have `icon1.png` and sound files in the directory):
   ```bash
   pyinstaller --noconsole --onefile --icon=icon1.png --name="FocusGuardPro" --add-data="icon1.png;." --add-data="*.wav;." --add-data="*.mp3;." main.py
   ```

---

## ⚙️ Configuration

FocusGuard Pro saves your preferences locally in `focus_config.json`. This file includes:
*   Theme settings (Opacity, Colors).
*   App blocklists and Profiles.
*   Session history.
*   Schedules.

**System Tray:** The app minimizes to the system tray. Double-click the tray icon to restore the window, or right-click to Quit.

---

## 🤝 Contributing

Contributions are welcome! If you find a bug or want to suggest a feature:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/NewFeature`).
3. Commit your changes.
4. Push to the branch and open a Pull Request.

---

## 👨‍💻 Author

**Mustafijur Rahman Ratul**
*   [GitHub](https://github.com/MustafijRatul)
*   [Facebook](https://www.facebook.com/share/1BsBPTF5DK/)

---

*This project is for educational and productivity purposes.*
