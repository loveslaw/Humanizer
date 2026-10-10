# 🎭 Humanizer - Discord Profile Customization & Warming Automation

A robust, multi-threaded automation tool designed to humanize, warm up, and customize Discord account tokens by batch updating avatars, profile banners, bio descriptions, pronouns, and activity states.

---

## ✨ Features
- **Profile Picture (PFP) Randomizer**: Automatically assigns unique profile pictures from an extensive high-quality avatar library.
- **Banner Customization**: Dynamically binds Nitro/non-Nitro banners to enhance account legitimacy.
- **Bio & Pronoun Formatter**: Injects varied biographies and pronouns from customizable datasets to reduce token similarity detection.
- **Proxy Support & Concurrency**: Integrates rotating HTTP/SOCKS proxies to bypass Cloudflare rate-limits and Discord IP flagging.
- **Automated Dependency Setup**: Included batch files (`setup.bat`, `start.bat`) for one-click environment installation.

---

## 📁 Repository Structure
```
Humanizer/
├── avatar/         # High-resolution avatar asset library
├── banners/        # Profile banner assets
├── data/           # Biographies, usernames, and status data presets
├── input/          # Target token input list and proxies
├── config.json     # Configuration file for threads, timeouts, and features
├── main.py         # Core multi-threaded humanization engine
├── req.txt         # Required Python dependencies
├── setup.bat       # Windows dependency installer
└── start.bat       # Windows launcher script
```

---

## 🚀 Installation & Setup

### Prerequisites
- Python 3.8+ installed on your system.

### Quick Start
1. Clone this repository:
   ```bash
   git clone https://github.com/loveslaw/Humanizer.git
   cd Humanizer
   ```
2. Install dependencies:
   ```bash
   pip install -r req.txt
   ```
   *(Or run `setup.bat` on Windows)*

3. Configure your tokens:
   - Place your Discord user tokens inside `input/tokens.txt`.
   - Optionally place proxies in `input/proxies.txt`.

4. Run the humanizer:
   ```bash
   python main.py
   ```
   *(Or launch via `start.bat`)*

---

## ⚙️ Configuration
Edit `config.json` to adjust:
- `threads`: Number of parallel concurrent worker threads.
- `change_avatar`: Toggle avatar updating.
- `change_bio`: Toggle bio customization.
- `change_banner`: Toggle banner updates.
- `delay`: Cooldown interval between account updates.

---

## ⚠️ Disclaimer
This tool is intended strictly for educational, security auditing, and account management research purposes. Ensure compliance with Discord's Terms of Service.
