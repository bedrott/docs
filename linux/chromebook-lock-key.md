# Chromebook Lock Key Integration (Hyprland + Noctalia)
To map the native Chromebook Overview / Switcher key (the rectangle with vertical bars on the right side of F4/Fullscreen) to trigger the Noctalia lock screen in Hyprland, follow these steps:
## Setup Guide

### Verify your Key Name:
Run wev in your terminal and press the Overview key to confirm it registers as XF86LaunchA.
### Add the Keybinding:
Open your Hyprland configuration file (~/.config/hypr/hyprland.lua) and add the following line under your keybindings section:

```
hl.bind("XF86LaunchA", hl.dsp.exec_cmd("noctalia msg session lock"))
```
Save the file. Press the Overview key on your keyboard, the Noctalia lock screen will trigger immediately.
