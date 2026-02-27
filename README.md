<p align="center">
  <img src="assets/icon.svg" alt="Arctic ComfyUI Helper" width="148" />
</p>

<h1 align="center">Arctic ComfyUI Helper</h1>

<p align="center">
  For users who want to install and manage ComfyUI with different add-ons and custom nodes very easily on Windows and Linux, plus get the right models and LoRAs without guesswork.
</p>

<p align="center">
  <a href="#"><img alt="Windows" src="https://custom-icon-badges.demolab.com/badge/Windows-0078D6?logo=windows11&logoColor=white" /></a>
  <a href="#"><img alt="Ubuntu" src="https://img.shields.io/badge/Ubuntu-E95420?logo=ubuntu&logoColor=white" /></a>
  <a href="#"><img alt="Debian" src="https://img.shields.io/badge/Debian-A81D33?logo=debian&logoColor=fff" /></a>
  <a href="#"><img alt="Linux Mint" src="https://img.shields.io/badge/Linux%20Mint-87CF3E?logo=linuxmint&logoColor=fff" /></a>
  <a href="#"><img alt="Fedora" src="https://img.shields.io/badge/Fedora-51A2DA?logo=fedora&logoColor=fff" /></a>
  <a href="#"><img alt="Arch Linux" src="https://img.shields.io/badge/Arch%20Linux-1793D1?logo=arch-linux&logoColor=fff" /></a>
</p>

<p align="center">
  <a href="#"><img alt="Built With" src="https://img.shields.io/badge/Built%20With-232323" /></a>
  <a href="#"><img alt="Rust" src="https://img.shields.io/badge/Rust-%23000000.svg?e&logo=rust&logoColor=white" /></a>
  <a href="#"><img alt="Tauri" src="https://img.shields.io/badge/Tauri-24C8D8?logo=tauri&logoColor=fff" /></a>
</p>

---

## 📚 Overview

Think of it as:
- A built-in **ComfyUI installer** for desktop workflows (easy setup from inside the app)
- A curated model/LoRA catalog matched to your hardware tiers
- A one-click downloader that places assets into the correct ComfyUI folders

---

### New in Latest Version

- 🧪 **Added Hugging Face Xet mode** as an optional experimental downloader for faster model downloads
- 🗂️ **Shared-folder support is now easier:** you can define one shared models folder across multiple ComfyUI installs, and `extra_model_paths` setup is handled for you
- 🧭 **New Workflows tab:** download my tutorial workflows in one click directly into your ComfyUI workflows folder
- ⏳ **Smoother startup and updates** with clearer loading/update messages, cleaner logs, and more reliable version checking

---

## 🧩 Core Features

- 🛠️ **ComfyUI install module** (uv-managed Python + selectable add-ons/custom nodes)
- 🧠 **Tier-aware catalog** that filters by your GPU VRAM and system RAM
- 📦 **Auto-dependency downloads** (text encoders, CLIPs, upscalers, and other required files)
- 🗂️ **Smart file placement** into the correct ComfyUI subfolders
- 📈 **Live download progress** with active/completed transfer tracking
- 🔐 **Optional Civitai token support** for authenticated LoRA downloads
- 🖼️ **LoRA preview + metadata** in-app (description, triggers, creator link)
- ♻️ **Auto-update support** through GitHub Releases manifest
- 🧵 **System tray controls** to Start/Stop ComfyUI even when the main window is hidden

---

## 🧰 ComfyUI Installer Highlights

Inside the **ComfyUI** tab, you can:

- Select a base folder and install a fresh ComfyUI instance
- Manage an existing ComfyUI installation
- Use automatic Torch/CUDA recommendation based on detected NVIDIA GPU
- Override Torch stack manually from dropdown
- Toggle add-ons and custom nodes from UI

### Available Add-Ons

- SageAttention
- SageAttention3 (RTX 50-series only)
- FlashAttention
- InsightFace
- Nunchaku
- Trellis2 (requires Torch 2.8.0 + cu128 or newer)
- Pinned Memory (enabled by default)

### Available Custom Nodes

- comfyui-manager
- ComfyUI-Easy-Use
- rgthree-comfy
- ComfyUI-GGUF
- comfyui-kjnodes

---

## 🚀 Getting Started

1. Download the latest package from this repo's **Releases** page:
   - Windows: `.exe`
   - Ubuntu / Debian / Linux Mint: `.deb`
   - Fedora: `.rpm`
   - Arch Linux: install from AUR: [`arctic-comfyui-helper-bin`](https://aur.archlinux.org/packages/arctic-comfyui-helper-bin)
2. Install it based on your distribution:
   - Windows:
     - No installation needed. Run the `.exe` directly (standalone app).
   - Ubuntu / Debian / Linux Mint:
     - `sudo apt install ./Arctic-ComfyUI-Helper_*.deb`
   - Fedora:
     - `sudo dnf install ./Arctic-ComfyUI-Helper-*.rpm`
   - Arch Linux:
     - `yay -S arctic-comfyui-helper-bin`
     - Or with paru: `paru -S arctic-comfyui-helper-bin`
3. Run the app. It is a **standalone desktop app**.
4. In **ComfyUI** tab, use **Install New** (or **Manage Existing**) if you want the app to install/manage ComfyUI itself.
5. In **Models** / **LoRAs**, select your existing ComfyUI folder to download assets.
6. Optional advanced logging: launch from terminal with `--nerdstats`  
   Examples: `.\Arctic-ComfyUI-Helper.exe --nerdstats` (Windows), `./Arctic-ComfyUI-Helper --nerdstats` (Linux)

That is it. Pick your setup, click, and the app handles the rest.

---

## 🖼️ Demo Preview

![Arctic Downloader Demo](assets/demo.png)

---

## 🔄 Auto-Updates

On startup, the app checks:

the latest update manifest from this repository's GitHub Releases.

If a newer version is found, the app downloads, verifies checksum, replaces binary, and restarts.

---

## ✅ Requirements

- Latest NVIDIA drivers installed
- Internet connection (for catalog, model files, and optional installer tasks)
- For some Civitai LoRAs: a valid Civitai API token

---

## 💡 Usage Tips

- If a LoRA says unauthorized, add your Civitai token in-app and save it.
- If you run multiple ComfyUI installs, use the ComfyUI tab's install/manage mode and detected installs list.

---

## 🆘 Need Help?

Open `Issues` -> `New issue`, then choose:
- **Cross-Platform Bug Report** for problems and errors
- **Feature Request** for ideas and improvements

Include:
- Platform and version (Windows or Linux distro/version)
- Package type used (`.exe`, `.deb`, `.rpm`, or AUR package `arctic-comfyui-helper-bin`)
- What you clicked
- What you expected
- What happened
- Any log lines shown in the app
- If possible, run with `--nerdstats` and include the exact terminal logs

---

## 🙏 Special Thanks

Thanks to [visualbruno](https://github.com/visualbruno) for the Trellis2 wrapper:  
https://github.com/visualbruno/ComfyUI-Trellis2

---

## 🛡️ VirusTotal

https://www.virustotal.com/gui/file/df11eb549dde404ddb6e0a73a5c9d61b1d1eecd11034dd9baa6d8b724b4e1121/detection

---

## 🧊 Author

Burce Boran 🎥 Asset Supervisor / VFX Artist | 🐧 Arctic Latent

[![YouTube – Arctic Latent](https://img.shields.io/badge/YouTube-%40ArcticLatent-FF0000?logo=youtube&logoColor=white)](https://youtube.com/@ArcticLatent)
[![Patreon – Arctic Latent](https://img.shields.io/badge/Patreon-Arctic%20Latent-FF424D?logo=patreon&logoColor=white)](https://patreon.com/ArcticLatent)
[![Hugging Face – Arctic Latent](https://img.shields.io/badge/HuggingFace-Arctic%20Latent-FFD21E?logo=huggingface&logoColor=white)](https://huggingface.co/arcticlatent)
[![Vimeo – Demo Reel](https://img.shields.io/badge/Vimeo-Demo%20Reel-1ab7ea?logo=vimeo&logoColor=white)](https://vimeo.com/1044521891)

---

## Support Project

[![Buy Me a Coffee – Arctic Latent](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-Arctic%20Latent-FFDD00?logo=buymeacoffee&logoColor=000)](https://buymeacoffee.com/arcticlatent)

---

## Open Source

This project is open source.

Development repositories:
- Linux: https://github.com/ArcticLatent/ArcticDownloader-lin
- Windows: https://github.com/ArcticLatent/ArcticDownloader-win
