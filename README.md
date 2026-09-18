# Snap64Recomp - Play Pokémon Snap Natively on PC

## 🚀 Getting Started

[![Download Snap64Recomp](https://img.shields.io/badge/Download-Snap64Recomp-blue?style=for-the-badge&logo=github)](https://github.com/harshithmothilal/Snap64Recomp)

Welcome! Snap64Recomp brings the classic Nintendo 64 game Pokémon Snap to your Windows or Linux computer. This version plays exactly like the original cartridge right out of the box, with no modifications needed. Every extra feature is completely optional and turned off by default, so purists get the authentic experience while curious players can explore enhancements later.

## 📥 Download and Install

Visit this link to download the application: [https://github.com/harshithmothilal/Snap64Recomp](https://github.com/harshithmothilal/Snap64Recomp)

The download page shows the latest release files. Look for the file named `Snap64Recomp-Windows.zip` (or similar) and click it to download. The file is about 10-15 MB, so it should download quickly on most connections.

If you are on Linux, look for `Snap64Recomp-Linux.tar.gz` instead. Steam Deck users should download the Linux version as well.

## 🖥️ System Requirements

Snap64Recomp is surprisingly light on resources, making it playable on a wide range of hardware. Here is what you need:

- **Operating System:** Windows 10 or newer, or a modern Linux distribution (Ubuntu 20.04+, Fedora 34+, SteamOS on Steam Deck)
- **Processor:** Any dual-core CPU from the past 10 years. Intel Core i3 or AMD Ryzen 3 or better recommended.
- **Memory:** 2 GB RAM minimum, 4 GB recommended.
- **Graphics:** Any GPU from the past 10 years. Integrated graphics like Intel HD 4000 or newer work fine. Dedicated GPUs recommended for higher resolution scaling.
- **Storage:** 50 MB free space for the application. You will also need space for your game dump (see below).
- **Display:** 800x600 resolution minimum, but the game supports up to 4K natively.

These are guidelines rather than hard limits, so older systems may still work. The emulation layer (called RT64) is highly optimized.

## 🕹️ Getting Your Game File

Snap64Recomp does not include any Nintendo game data, so you need to provide your own copy of Pokémon Snap for the N64. This is called a "ROM dump" or just a "dump."

Here is what you need:

1. **A Pokémon Snap N64 cartridge.** You likely have this if you owned the game. If not, check retro game stores or online marketplaces.
2. **A way to read the cartridge.** Many USB N64 cartridge readers are available online for around $30-50. Look for one that mentions "ROM dumping" capability.
3. **The extracted ROM file.** After dumping, you should have a file ending in `.z64` or `.n64`. This is the file Snap64Recomp needs.

Alternatively, if you own a Wii Virtual Console copy of Pokémon Snap, you can extract the ROM from that using homebrew tools, though this is a bit more technical.

Place this ROM file in the same folder as your Snap64Recomp application. The program will find it automatically when you launch the game.

## ⚙️ First Launch

1. Double-click `Snap64Recomp.exe` (Windows) or run `./Snap64Recomp` from a terminal (Linux/Steam Deck).
2. The game will scan for your ROM file. If it finds multiple versions, it will ask you which one to use. Pick the one that matches your cartridge region (NTSC for US/Japan, PAL for Europe).
3. The main menu appears. From here, you can also change options if you want.
4. The game runs at its original resolution by default (320x240). Everything will look blocky and sharp like the real N64. That is intentional.

That is it! You are now playing Pokémon Snap on your computer.

## 🎮 Controls

The controls map directly to the N64 controller. Here is the default setup:

| Action | N64 Button | Keyboard | Xbox Controller | PlayStation Controller |
|--------|------------|----------|-----------------|----------------------|
| Move | Control Stick | WASD | Left Stick | Left Stick |
| Camera Up | C-Up | Up Arrow / I | Right Stick Up / Y | Right Stick Up / Triangle |
| Camera Down | C-Down | Down Arrow / K | Right Stick Down / A | Right Stick Down / X |
| Camera Left | C-Left | Left Arrow / J | Right Stick Left / X | Right Stick Left / Square |
| Camera Right | C-Right | Right Arrow / L | Right Stick Right / B | Right Stick Right / Circle |
| Take Photo | A | Space / Enter | A | X |
| Feed Apple | B | Shift / Z | B | Circle |
| Use Pester Ball (L) | Z | Left Ctrl | Left Trigger | L1 |
| Use Pester Ball (R) | R | Right Ctrl | Right Trigger | R1 |
| Pause | Start | Esc / P | Start | Options |

You can change these in the Settings menu if something feels wrong.

## 🔧 Optional Enhancements

While Snap64Recomp is 100% authentic by default, we included some opt-in features for those who want them. None of these change the game logic, but they improve visual quality or comfort. Enable them from the in-game Settings menu.

### High Resolution Rendering
Renders the game at your monitor's native resolution instead of 320x240. The graphics become much sharper. Every texture stays the same, but geometric edges smooth out significantly.

### Widescreen Support
Changes the viewport from the original 4:3 aspect ratio to 16:9 or 21:9. Note that this reveals areas outside the original camera bounds. Some object placements look odd since the developers never intended those areas visible. This is purely cosmetic and completely optional.

### Texture Filtering
Smooths out the pixelated textures. This mimics how the game looked in early emulator screenshots or on CRT TVs with a blurry signal, but on modern displays it can make everything look slightly softer. Many players prefer this for readability.

### Improved Draw Distance
Pushes the far clipping plane further away. This means distant objects and Pokémon appear sooner instead of popping into view. It does not alter gameplay but reduces visual distractions.

### Cheat Codes
A selection of official-style GameShark codes is included. Things like "Always Show Pokémon", "Infinite Film", and "Unlock All Levels" are available. These are entirely on by default, so you must manually enable them.

## 🐛 Troubleshooting

**Game will not start**
Check that your ROM file is in the same folder and named correctly. The file should end in `.z64` or `.n64`. If you have multiple Pokémon Snap ROMs, only keep one in the folder.

**Game runs slowly**
Your system may not meet the recommended specs. Close other programs and try a lower-resolution setting. You can also switch to the software renderer in advanced options.

**No sound**
Ensure your audio drivers are up to date. Try changing the audio backend option in Settings from Automatic to your specific device.

**Steam Deck controls not working**
Switch the control scheme in the in-game Options menu to "Gamepad". If issues persist, restart the game after changing the setting.

**Graphics look wrong or glitchy**
Your GPU driver might not support modern Vulkan features. Update your graphics driver, then go to Advanced Settings and switch the Renderer from Vulkan to Direct3D 12 (Windows) or OpenGL (Linux).

## ❓ Frequently Asked Questions

**Do I need an N64 controller?**
No. Keyboard and any modern gamepad work out of the box.

**Can I play with friends?**
Pokémon Snap was a single-player game and remains so in this port.

**Is online multiplayer possible?**
No. There is no multiplayer mode in any version of this game.

**Can I use my save files from an N64 cartridge?**
Not directly. However, you can use a memory card reader to extract your save data, then use the "Import Save" option in Settings. This process is manual and may require technical tools.

**Will this work on Mac?**
Currently only Windows and Linux are supported. Compatibility layers like Wine or CrossOver might work, but we do not officially support them.

**How is this different from using an emulator?**
Snap64Recomp converts the original N64 code into native PC code once, so it runs much faster and more efficiently than a real-time emulator. There is no performance overhead, and input latency is lower. It also integrates directly with modern graphics APIs.

## 📸 Screenshots

(Placeholder text: Include 3-4 screenshots here showing the game running at high resolution, widescreen, and the original look. In the real README, you would drop image files here.)

## 📜 License and Legal

Snap64Recomp is released under the MIT License. The original Pokémon Snap game is copyrighted by Nintendo. This project does not distribute any copyrighted material. You must own a legitimate copy of Pokémon Snap to use this application.

This project is for preservation and educational purposes. No affiliation with Nintendo.

## 🤝 Contributing

We welcome bug reports and feature requests through the GitHub Issues page. If you want to contribute code, see the CONTRIBUTING.md file in the repository.

If you enjoy Snap64Recomp, consider starring the repository so more people discover this preservation effort.

## 🔗 Related Projects

- [N64Recomp](https://github.com/N64Recomp/N64Recomp) – The framework that makes this possible
- [RT64](https://github.com/N64Recomp/RT64) – The real-time rendering engine used

Keywords: linux, n64, n64recomp, nintendo-64, pokemon, pokemon-snap, recompilation, rt64, static-recompilation, steam-deck, windows