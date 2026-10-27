# 📱 Omni Terminal

> **Custom Android Terminal Workstation running the OMNI Command & Control Suite.**  
> *Built on top of the open-source Termux platform, tuned for mobile productivity, AI assistance, and seamless multi-device orchestration.*

Author: **Jordan Isaac ([@dragpk247](https://github.com/dragpk247))**  
License: **GPL-v3.0**

---

## ⚡ Overview

**Omni Terminal** is an Android terminal emulator and Linux environment customized to serve as the mobile command center for the **[Omni CLI](https://github.com/dragpk247/omni-cli)** ecosystem.

Whether you are triggering AI coding agents, streaming commands to your Linux desktop/laptop, syncing clipboards, or transferring files over Tailscale, Omni Terminal provides a dedicated mobile workstation on your phone.

---

## ✨ Features

- **Built for Omni CLI**: Seamlessly runs `omni`, `omni-phone`, and the rest of the Omni fleet utilities out of the box.
- **Hardware & Battery Sentinel**: Protects mobile hardware by monitoring thermals and battery levels during intensive tasks.
- **Universal Clipboard & File Sharing**: Full compatibility with `omni clip` and `omni send` over local networks and Tailscale.
- **Mobile AI Copilot**: Direct terminal-based voice and text AI interactions (`omni ask`, `omni voice`).
- **Full Linux Userland**: Powered by apt/pkg package management, Zsh/Bash, Git, Python, Node.js, OpenSSH, and Neovim.

---

## 📲 Installation

### Option 1: GitHub Releases (Recommended)
1. Download the latest `OmniTerminal.apk` from [Releases](https://github.com/dragpk247/omni-terminal/releases).
2. Install the APK on your Android device (ensure "Install unknown apps" is granted for your browser/installer).
3. Open Omni Terminal and allow storage permissions when prompted.

### Option 2: Building from Source
```bash
git clone https://github.com/dragpk247/omni-terminal.git
cd omni-terminal
./gradlew assembleDebug
```
The compiled APK will be located at `app/build/outputs/apk/debug/app-debug.apk`.

---

## 🚀 Getting Started

Once inside Omni Terminal, set up your Omni environment:

```bash
# 1. Install or update Omni CLI
curl -fsSL https://raw.githubusercontent.com/dragpk247/omni-cli/main/install.sh | bash

# 2. Run the interactive setup
omni setup

# 3. Launch the mobile dashboard
omni
```

---

## 🔗 Companion Repositories

- **[omni-cli](https://github.com/dragpk247/omni-cli)**: Core CLI orchestrator bridging Desktop, Laptop, and Phone.
- **[dotfiles](https://github.com/dragpk247/dotfiles)**: Personal configurations and system scripts.

---

## 📜 Credits & Upstream

Omni Terminal is built upon the foundational work of the **[Termux](https://github.com/termux/termux-app)** project and community.
Licensed under the GNU General Public License v3.0 (GPLv3).
