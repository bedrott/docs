# How to install Sober on Linux
Quick guide to install Sober (Roblox client for Linux) via Flatpak on any distribution.

## 1. Install Flatpak

Choose the command for your Linux distribution:

Ubuntu / Linux Mint / Pop!_OS / Debian:
```bash
sudo apt update && sudo apt install flatpak
```
Arch Linux / CachyOS / Manjaro:
```bash
sudo pacman -S flatpak
```
Fedora:
```bash
sudo dnf install flatpak
```
## 2. Add Flathub Repository
```bash
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```
(Optional: Reboot your system after this step to make sure application shortcuts show up properly).

## 3. Install Sober
```bash
flatpak install flathub org.vinegarhq.Sober
```
## 4. Run Sober

Launch Sober from your desktop application menu, or run it via terminal:
```bash
flatpak run org.vinegarhq.Sober
