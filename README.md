# althro's dwm build
My personal dwm build heavily inspired by [luke's build](https://github.com/lukesmithxyz/dwm)

## Patches and Features
- Clickable status bar with [dwmblocks](https://github.com/throal/dwmblocks)
- Xresources and pywal support
- New layouts: bstack, fibonacci, deck, centered master and more. All bound to keys `super+(shift+)t/y/u/i`
- scratchpads: (`super+shift+enter`)
- actualfullscreen: toggle fullscreen for a window (`super+f`)
- sticky: make client visible on all tags (`super+s`)
- stacker: move the windows up the stack manually (`super+K/J`)
- swallow: this patch helps users spawning a lot of graphical programs from their command line by avoiding cluttering the screen with many unusable terminals.
- pertag: this patch keeps layout, mwfact, barpos and nmaster per tag.

## Installation
```
git clone https://github.com/throal/dwm
cd dwm
sudo make install
```

### Please install `libxft-bgra`!
This build of dwm does not block color emoji in the status/info bar, so you must install [libxft-bgra](https://aur.archlinux.org/packages/libxft-bgra/) from the AUR, which fixes a libxft color emoji rendering problem, otherwise dwm will crash upon trying to render one. Hopefully this fix will be in all libxft soon enough.
