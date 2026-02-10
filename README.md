<p align="center">
  <img src="assets/icon.svg" alt="Arctic ComfyUI Helper" width="148" />
</p>

<h1 align="center">Arctic ComfyUI Helper</h1>

<p align="center">
  A curated Windows companion for ComfyUI users who want the right models, LoRAs, and setup tools without guesswork.
</p>

<p align="center">
  <img alt="Windows" src="https://img.shields.io/badge/Platform-Windows%2010%2F11-0078D4?style=for-the-badge&logo=windows&logoColor=white" />
  <img alt="Rust" src="https://img.shields.io/badge/Built%20with-Rust-000000?style=for-the-badge&logo=rust" />
  <img alt="Tauri" src="https://img.shields.io/badge/Desktop-Tauri-24C8DB?style=for-the-badge&logo=tauri&logoColor=white" />
</p>

---

## 📚 Overview

Arctic ComfyUI Helper mirrors the exact builds shown in Arctic Latent tutorials, so you can follow along with less setup friction.

Think of it as:
- A built-in **ComfyUI installer** for Windows (easy setup from inside the app)
- A curated model/LoRA catalog matched to your hardware tiers
- A one-click downloader that places assets into the correct ComfyUI folders

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

1. Download the latest `Arctic-ComfyUI-Helper.exe` from this repo's **Releases** page.
2. Run the app.
3. In **Models** / **LoRAs**, select your existing ComfyUI folder to download assets.
4. In **ComfyUI** tab, use **Install New** (or **Manage Existing**) if you want the app to install/manage ComfyUI itself.

That is it. Pick your setup, click, and the app handles the rest.

---

## 🔄 Auto-Updates

On startup, the app checks:

`https://github.com/ArcticLatent/Arctic-Helper/releases/latest/download/update.json`

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

Open an issue in this repository with:
- What you clicked
- What you expected
- What happened
- Any log lines shown in the app

---

## 🧊 Author

Burce Boran 🎥 Asset Supervisor / VFX Artist | 🐧 Arctic Latent

[![YouTube – Arctic Latent](https://img.shields.io/badge/YouTube-%40ArcticLatent-FF0000?logo=youtube&logoColor=white)](https://youtube.com/@ArcticLatent)
[![Patreon – Arctic Latent](https://img.shields.io/badge/Patreon-Arctic%20Latent-FF424D?logo=patreon&logoColor=white)](https://patreon.com/ArcticLatent)
[![Hugging Face – Arctic Latent](https://img.shields.io/badge/HuggingFace-Arctic%20Latent-FFD21E?logo=huggingface&logoColor=white)](https://huggingface.co/arcticlatent)
[![Vimeo – Demo Reel](https://img.shields.io/badge/Vimeo-Demo%20Reel-1ab7ea?logo=vimeo&logoColor=white)](https://vimeo.com/1044521891)

---

Copyright (c) 2026 Arctic Helper. All Rights Reserved.

This software is proprietary and closed-source.

You may download and use for personal use only. Redistribution, modification, reverse engineering, or commercial use of this software or any included assets is prohibited without written permission from the copyright holder.

The software is provided “as is” without warranty of any kind.
