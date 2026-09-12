# How to Map the Chromebook Fullscreen Key in Hyprland (Lua Config)

## If you are using Hyprland with a Lua configuration file (hyprland.lua) on a Chromebook, follow these steps to make the native fullscreen key work:

Open your configuration file in a terminal text editor:
```
nano ~/.config/hypr/hyprland.lua
```
Locate the Keybindings section inside the file:

### 3. **Add the keybinding rule** under that section:
```
hl.bind("XF86Fullscreen", hl.dsp.window.fullscreen())
```

(Note: If your specific Chromebook model maps this key to F11 instead, replace "XF86Fullscreen" with "F11").

Save the file and exit (Ctrl + O, Enter, then Ctrl + X in nano).

Hyprland will reload your configuration automatically, allowing you to toggle fullscreen mode instantly using your Chromebook's dedicated key.

Thank You :)
