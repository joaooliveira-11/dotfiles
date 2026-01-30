# 🗂️ Dotfiles

My personal dotfiles for macOS, managed with [GNU Stow](https://www.gnu.org/software/stow/). It includes personal configurations for Ghostty, Aerospace and NeoVim (soon), among others.

## 📦 What's Included

| Tool | Description |
|------|-------------|
| [Aerospace](#-aerospace) | Tiling window manager for macOS |
| [Tmux](#-tmux) | Terminal multiplexer |
| [Starship](#-starship) | Cross-shell prompt |
| [Ghostty](#-ghostty) | GPU-accelerated terminal emulator |
| [Sketchybar](#-sketchybar) | Custom macOS menu bar |
| [Borders](#-borders) | Window border highlighting |

---

## 🚀 Installation

### Prerequisites

```bash
# Install Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install GNU Stow
brew install stow
```

### Core Tools

```bash
# Window management & UI
brew install --cask aerospace ghostty
brew install tmux sketchybar borders

# Shell prompt
brew install starship

# Shell enhancements
brew install zsh-autosuggestions zsh-syntax-highlighting

# Modern CLI replacements
brew install eza        # Better ls
brew install bat        # Better cat
brew install fd         # Better find
brew install fzf        # Fuzzy finder
brew install zoxide     # Smarter cd
```

### Optional Tools

```bash
brew install neovim     # Terminal editor (when ready)
```

### Setup

```bash
# Clone the repository
git clone https://github.com/joaooliveira-11/dotfiles ~/dotfiles

# Navigate to dotfiles directory
cd ~/dotfiles

# Stow everything (creates symlinks to ~)
stow -t ~ .
```

> [!NOTE]
> The `-t ~` flag tells stow to create symlinks in your home directory.
> This will symlink `.config/`, `.zshrc`, `.gitconfig`, etc. to `~`.

---

## 🪟 Aerospace

[Aerospace](https://github.com/nikitabobko/AeroSpace) is an i3-like tiling window manager for macOS.

### App Launchers

| Shortcut | Action |
|----------|--------|
| `Alt + B` | Open Google Chrome |
| `Alt + T` | Open Ghostty (Terminal) |
| `Alt + N` | Open Notion |
| `Alt + C` | Open Notion Calendar |
| `Alt + Z` | Open Zotero |
| `Alt + S` | Open Slack |
| `Alt + D` | Open Discord |
| `Alt + W` | Open WhatsApp |
| `Alt + G` | Open ChatGPT |

### Window Navigation

| Shortcut | Action |
|----------|--------|
| `Alt + H` | Focus window left |
| `Alt + J` | Focus window down |
| `Alt + K` | Focus window up |
| `Alt + L` | Focus window right |
| `Alt + Tab` | Switch to previous workspace |

### Window Movement

| Shortcut | Action |
|----------|--------|
| `Alt + Shift + H` | Move window left |
| `Alt + Shift + J` | Move window down |
| `Alt + Shift + K` | Move window up |
| `Alt + Shift + L` | Move window right |

### Layout & Sizing

| Shortcut | Action |
|----------|--------|
| `Alt + E` | Toggle tiles layout (horizontal/vertical) |
| `Alt + ,` | Toggle accordion layout |
| `Alt + F` | Toggle fullscreen |
| `Alt + Shift + -` | Shrink window |
| `Alt + Shift + =` | Expand window |

### Workspaces

| Shortcut | Action |
|----------|--------|
| `Alt + 1-7` | Switch to workspace 1-7 |
| `Alt + Shift + 1-7` | Move window to workspace 1-7 |
| `Alt + Shift + Tab` | Move workspace to next monitor |

### Code Mode (`Alt + Shift + C`)

| Shortcut | Action |
|----------|--------|
| `P` | Open PyCharm |
| `V` | Open VS Code |
| `A` | Open Antigravity |
| `W` | Open WebStorm |
| `R` | Open Rider |
| `Esc` | Exit code mode |

### Service Mode (`Alt + Shift + ;`)

| Shortcut | Action |
|----------|--------|
| `Esc` | Reload config & exit |
| `R` | Reset/flatten workspace layout |
| `F` | Toggle floating/tiling |
| `Backspace` | Close all windows but current |

### Default Workspace Assignments

| App | Workspace |
|-----|-----------|
| Chrome | 1 |
| Antigravity, PyCharm | 2 |
| Ghostty | 3 |
| Notion | 4 |
| Slack, Discord, WhatsApp | 5 |

---

