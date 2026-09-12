# Display Brightness Control

## Install the brightness utility:
```
sudo pacman -S brightnessctl
```
### Add the binding rules to your ~/.config/hypr/hyprland.lua:
```
hl.bind("XF86MonBrightnessUp",  hl.dsp.exec_cmd("brightnessctl set +5%"), { locked = true, repeating = true })
hl.bind("XF86MonBrightnessDown",hl.dsp.exec_cmd("brightnessctl set 5%-"), { locked = true, repeating = true })
```
