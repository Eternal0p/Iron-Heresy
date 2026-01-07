# Iron Heresy - Godot Setup Guide

## Installing Godot

Since Godot is not currently installed on your system, follow these steps:

### Option 1: Download Standard Version (Recommended)
1. Visit the official Godot website: https://godotengine.org/download/windows/
2. Download **Godot 4.x (Standard version)** - The latest stable release
3. Extract the ZIP file to a folder (e.g., `C:\Godot`)
4. Run `Godot_v4.x_win64.exe`

### Option 2: Download via Steam
1. Open Steam
2. Search for "Godot Engine"
3. Download and install (it's free!)

### Option 3: Download .NET Version (If you want C# support)
1. Visit: https://godotengine.org/download/windows/
2. Download **Godot 4.x (.NET version)**
3. Requires .NET SDK 6.0 or later

---

## Creating Your Iron Heresy Project

Once Godot is installed:

1. **Launch Godot**
   - Run the Godot executable

2. **Create New Project**
   - Click "New Project"
   - Project Name: `Iron Heresy`
   - Project Path: `c:\Users\airbo\Desktop\Eternal\Iron-Heresy`
   - Renderer: Select "Forward+" (best for 2D with effects) or "Mobile" (lighter)
   - Click "Create & Edit"

3. **Configure Project Settings**
   - Go to `Project → Project Settings`
   - **Display → Window:**
     - Width: 1280
     - Height: 720
     - Mode: Windowed
     - Resizable: On
     - Aspect: Keep
   - **Rendering → Textures:**
     - Default Texture Filter: Nearest (for pixel art)

4. **Set Up 2D Scene**
   - Click "2D" at the top
   - This is your main workspace

---

## Project Structure Already Created ✓

The following folder structure has been set up for you:

```
Iron-Heresy/
├── assets/
│   ├── sprites/
│   │   ├── player/       # Player character sprites
│   │   ├── enemies/      # Enemy sprites
│   │   ├── environment/  # Tiles, backgrounds, props
│   │   ├── ui/          # UI elements
│   │   └── vfx/         # Visual effects
│   ├── audio/
│   │   ├── music/       # Background music
│   │   └── sfx/         # Sound effects
│   └── tilesets/        # Tileset files
├── scripts/
│   ├── player/          # Player-related scripts
│   ├── enemies/         # Enemy AI scripts
│   ├── systems/         # Core game systems
│   └── ui/              # UI scripts
├── scenes/
│   ├── levels/          # Level scenes
│   ├── ui/             # UI scenes
│   ├── player/         # Player scene
│   └── enemies/        # Enemy scenes
├── GDD.md              # Game Design Document
└── DEVELOPMENT_CHECKLIST.md
```

---

## Recommended Additional Tools

### For Pixel Art
- **Aseprite** ($19.99): https://www.aseprite.org/
  - Industry standard for pixel art
  - Built-in animation tools
- **Piskel** (Free): https://www.piskelapp.com/
  - Online pixel art editor
  - Export as sprite sheets

### For Audio
- **Audacity** (Free): https://www.audacityteam.org/
  - Audio editing and sound effects
- **LMMS** (Free): https://lmms.io/
  - Music composition
- **Bosca Ceoil** (Free): https://boscaceoil.net/
  - Simple music creation for games

### For Level Design
- **Tiled** (Free): https://www.mapeditor.org/
  - Create tilemaps
  - Export to Godot format

---

## Next Steps

1. ✅ Install Godot
2. ✅ Create Iron Heresy project in Godot
3. ✅ Configure project settings
4. 📝 Fill out the GDD.md (Game Design Document)
5. 🎨 Start creating pixel art assets
6. 💻 Begin prototyping (when you're ready!)

---

## Quick Start After Installation

Once Godot is set up, you can:
1. Import your assets into the respective folders
2. Create your first scene (Player character)
3. Start scripting basic movement
4. Test in the Godot editor with F5

**Need help with any of these steps? Just let me know!**
