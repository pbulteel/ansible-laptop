# ansible-laptop

Ansible playbook to set up a laptop with commonly used applications and development tools.

## Usage

```bash
ansible-playbook laptop.yml
```

Run with specific tags:
```bash
ansible-playbook laptop.yml --tags "nvm,docker"
```

## What's Installed

### Repositories Added
- Google Chrome
- Microsoft (VS Code, Edge)
- HashiCorp (Vault, Terraform, Packer)
- Kubernetes (kubectl)
- Docker
- GitHub CLI
- Steam
- MEGA
- Lutris
- KeePassXC (via Flatpak)

### Core Development Tools
- git, vim, build-essential
- curl, wget, unzip
- tmux, byobu
- python3-pip, python3-venv

### Modern CLI Tools
- **fzf** - Fuzzy finder for files/commands
- **ripgrep (rg)** - Fast grep alternative
- **fd-find (fd)** - Fast find alternative
- **bat** - Cat with syntax highlighting
- **jq** - JSON processor
- **yq** - YAML processor
- **tree** - Directory listing
- **htop** - Process viewer
- **nmap** - Network scanner

### Container & Orchestration
- **Docker** - Container runtime with compose plugin
- **kubectl** - Kubernetes CLI

### Node.js
- **nvm** - Node Version Manager
- **Node.js LTS** - Latest LTS version via nvm

### Applications (via apt)
- Google Chrome, Microsoft Edge
- VS Code
- VLC, GIMP, Inkscape, Blender
- Flameshot, Shutter, Peek (screenshots)
- Nextcloud Desktop
- Remmina (RDP/VNC client)
- Wireshark, nmap
- htop, iftop

### Applications (via Snap)
- Spotify, Slack, Telegram
- Postman, Audacity
- Spotify, Calibre
- Powershell
- And more...

### Applications (via Flatpak)
- DBeaver Community (database tool)
- KeePassXC (password manager)
- Draw.io Desktop
- Clementine (music player)

### VPN & Remote
- OpenFortiVPN
- NSG VPN (work-specific)

### Gaming
- Steam, Lutris
- 0 A.D. (via snap)

## Tags

Use tags to run specific parts of the playbook:

- `packages` - Core apt packages
- `nvm` / `node` - Node.js via nvm
- `docker` - Docker installation
- `github-cli` / `gh` - GitHub CLI
- `hashicorp` - Vault, Terraform, Packer
- `kubectl` - Kubernetes CLI
- `chrome` - Google Chrome
- `microsoft` - VS Code, Edge
- `snap` - Snap packages
- `flatpak` - Flatpak packages
- `updates` - System update/upgrade
