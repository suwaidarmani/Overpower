# Overpower# Overpower Legends: Dungeon Clash

## Introduction
"Overpower Legends: Dungeon Clash" is an action RPG arena fighting game that combines elements from popular anime like Naruto, Solo Leveling, Dragon Ball, One Piece, and more. This game is optimized for low-end Android devices with a size under 300MB while maintaining HD graphics and smooth gameplay. The game is built using Godot 4 with GDScript, and it can be automated using Termux on Android.

## Features

### Name
**Overpower Legends: Dungeon Clash**

### Genre & Gameplay
- Arena Fighting + RPG + MOBA
- Combines concepts from Naruto Storm and Solo Leveling
- Fast-paced movement with dodge, block, and counter-attack mechanics
- Combo system with cinematic ultimate skill effects

### Engine & Coding
- **Godot 4 + GDScript** (Lightweight and compatible with Termux)
- **Pygame + Python** (Alternative for ultra-lightweight game)

### Platform & Performance
- **Android** (Support for Low-End & High-End, optimized for 30FPS & 60FPS)
- **PC** (Exportable to Windows if needed)

### Size & Graphic Optimization
- Maximum 300MB
- Uses lightweight shaders & texture compression
- Lower resolution for Low-End but retains HD quality
- Skill effects using lightweight particle systems

### Multiplayer Mode
- PvP Online 1v1 & 5v5
- Co-op Dungeon Raid Mode
- AI Matchmaking System

### AI System (Adaptive & Override Mode)
- Enemy AI learns player fighting style
- Boss AI becomes stronger when HP is low
- AI Override Mode (Enemies can counter-attack based on battle history)

### Hero System & Unlockable Content
- Free Initial Hero: Jinwoo (Solo Leveling)
- Unlockable Heroes: Naruto, Goku, Gojo, Madara, Luffy, Dio, Erza, Saitama, etc.
- Each hero has an Awakening Mode & Ultimate Skill

### Monetization & Progression System
- In-App Purchase (Buy Heroes, Skins, Power-ups)
- Free-to-Play with Ads Reward
- XP Leveling to unlock skills & weapons


## Setup & Build Game in Termux (Automation)
Use Termux to build the game without needing a PC.

### 1. Install Termux & Dependencies
```sh
pkg update && pkg upgrade -y
pkg install git wget unzip clang python nodejs -y
```

### 2. Install Godot 4 Headless for Building the Game
```sh
wget https://downloads.tuxfamily.org/godotengine/4.x/Linux/Godot_v4.0-stable_linux_headless.64.zip
unzip Godot_v4.0-stable_linux_headless.64.zip
chmod +x Godot_v4.0-stable_linux_headless.64
mv Godot_v4.0-stable_linux_headless.64 ~/bin/godot
```

### 3. Clone Game Project & Run in Termux
```sh
git clone https://github.com/user/projek-game.git
cd projek-game
~/bin/godot --headless --project-manager
```

### 4. Build APK Automatically
```sh
~/bin/godot --export "Android" bin/overpower_legends.apk
```

## Conclusion
With this prompt, you can automatically build and optimize the game in Termux! If you need config XML files, APK splits, or a ready-to-use setup, let me know!
