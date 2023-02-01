## Install

### Base

- Archinstall with sway as desktop

### Yay

```
# Before this you need base-devel installed
git clone https://aur.archlinux.org/yay-bin
cd yay-bin
makepkg -si
```

## Packages

``` bash
yay -S swaybg swaync polkit alacritty wofi xorg-xwayland sddm-git neofetch thunar \
waybar jetbains-fleet Alacritty
```

### Optional

``` bash
yay -S xorg-xwayland
```
xorg-xwayland

## Env variables needed

```
export _JAVA_AWT_WM_NONREPARENTING=1 #java applications to work such as idea on wayland/xwayland
export MOZ_ENABLE_WAYLAND=1 #fix mozilla blury
```

### VMware

```
export WLR_NO_HARDWARE_CURSORS=1
export WLR_RENDERER_ALLOW_SOFTWARE=1
```

## Gotchas

- 3D Acceleration needs to be enabled for VMware to work with wayland

## Docs needed

- https://wiki.archlinux.org/title/SDDM

## Sources used making these
