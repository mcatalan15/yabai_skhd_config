# Yabai & SKHD Configurations for macOS

This repository contains my custom configurations for [Yabai](https://github.com/koekeishiya/yabai), a tiling window manager for macOS, and [SKHD](https://github.com/koekeishiya/skhd), a hotkey daemon for managing keyboard shortcuts.

## Getting Started

### Prerequisites

- **macOS**: Ensure you're using macOS for compatibility.
- **Homebrew**: Install Homebrew if needed:
  ```bash
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  ```

### Install Yabai & SKHD

1. Install Yabai:
   ```bash
   brew install koekeishiya/formulae/yabai
   ```

2. Install SKHD:
   ```bash
   brew install koekeishiya/formulae/skhd
   ```

### Setup

1. **Copy configuration files**:
   ```bash
   cp yabai/yabairc ~/.yabairc
   cp skhd/skhdrc ~/.skhdrc
   ```

2. **Enable Yabai scripting additions**:
   ```bash
   sudo yabai --install-sa
   sudo yabai --load-sa
   ```

3. **Start Yabai and SKHD**:
   ```bash
   brew services start yabai
   brew services start skhd
   ```

### Keybindings Overview

The `skhdrc` file includes custom keybindings for managing windows and displays. Some keybindings include:

- **Window focus**: `alt + j/k/h/l` to focus windows in different directions.
- **Display focus**: `alt + s/g` to focus external displays.
- **Window management**: `shift + alt` combined with keys for operations like toggle float, maximize, balance, and swap windows.
- **Space management**: Move windows between spaces using `shift + alt + [number]`.

