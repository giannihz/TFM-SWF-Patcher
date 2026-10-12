# 🧀 TFM SWF Patcher Suite

A ready-to-use, interactive binary patching tool for **Transformice client SWFs**. Easily redirect game connections, configure panel assets, replace official image servers, update branding, and customize links without needing to recompile ActionScript bytecode.

---

## 🚀 Features

- ⚡ **Direct Binary Patching:** Safe, surgical string replacements in the SWF string pool (CPOOL) while fully preserving bytecode structure.
- 🌐 **Network Redirections:**
  - Game server Host/IP and port.
  - Web panel server (avatars, forums, language files).
  - Atelier801 / Transformice image servers (`x_bibliotheques`, skins, chamanes, backgrounds).
- 🎨 **Branding & Visuals:**
  - In-game logo text replacement (`Transformice` ➔ Your Server Name).
  - Custom destination URL when players click the client logo.
  - Redirect the Steam sign/button to your community Discord or website.
- 💬 **Interactive Prompts:** Every setting asks for your input with sensible defaults. No forced hardcoded values.

---

## 📥 Where to Get the Latest Client SWF

You can always download the latest official client directly from the game servers:

- 🔗 **Direct Download Link:** [https://www.transformice.com/Transformice.swf](https://www.transformice.com/Transformice.swf)

Place the downloaded `Transformice.swf` file directly in the same directory as `TFM_Patcher.exe` before patching.

---

## 📦 What's Included

```text
TFM_SWF_Patcher/
├── TFM_Patcher.exe            # Pre-compiled standalone patcher
├── Transformice.swf           # Base client SWF ready to be patched
├── addons/                    # Auxiliary tools and debugging utilities
│   ├── ffdec-cli.jar          # Command-line SWF tool
│   ├── swfdump.exe            # Binary inspector
│   ├── flashplayer_debug.exe  # Standalone Flash Debugger player
│   └── ...                    # Assets and helper scripts
├── .gitignore
└── README.md
```

---

## 🛠️ Quick Start

1. Make sure `Transformice.swf` is in the same folder as `TFM_Patcher.exe`.
2. Run **`TFM_Patcher.exe`**.
3. Follow the 6 interactive prompts:
   - **Step 1:** Game server IP / Host & Port.
   - **Step 2:** Web panel redirect (forums, avatars, languages).
   - **Step 3:** Image server redirect (`/images/`).
   - **Step 4:** Steam sign link (Discord / Website URL).
   - **Step 5:** Client logo text & Click URL.
   - **Step 6:** Additional copy destination (optional).
4. The patched SWF will be saved automatically, and a timestamped backup of the original will be created in `SWF_YYYYMMDD_HHMMSS/`.

---

## 📄 License

This project is licensed under the **MIT License**. Free to use and adapt for Transformice private server development.
