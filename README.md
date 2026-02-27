# Toye-Cyberlabs Hacker Terminal Theme

Files added:
- `banner.txt` — ASCII login banner with specializations
- `prompt.sh` — Bash prompt (green-on-black) and environment variables
- `gnome-terminal-setup.sh` — Attempt to create a GNOME Terminal profile with palette
- `install.sh` — Copies files and adds sourcing to `~/.bashrc`

Also included:
- `alacritty.yml` — Alacritty color config (green-on-black)
- `kitty.conf` — Kitty color config

Quick install:
```bash
cd /path/to/repo/hacker-theme
./install.sh
source ~/.bashrc
```

Notes:
- `gnome-terminal-setup.sh` uses `gsettings`/`dconf`; it may require tweaks on some systems.
- The installer backs up `~/.bashrc` to `~/.bashrc.toye-backup` before editing.

Alacritty usage:
```bash
# copy into your config (overwrites colors section)
mkdir -p ~/.config/alacritty
cp alacritty.yml ~/.config/alacritty/alacritty.yml
```

Kitty usage:
```bash
# copy and include from your main kitty.conf
mkdir -p ~/.config/kitty
cp kitty.conf ~/.config/kitty/toye-cyberlabs.conf
# then add to ~/.config/kitty/kitty.conf:
# include toye-cyberlabs.conf
```
