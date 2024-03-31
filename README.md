# WIP! Come back in a day or so.
# Plasma 6 and i3: A Guide for 2024
Tested on EndeavourOS. Intended for people with Linux experience but not i3 experience. Inspired by [this](https://github.com/heckelson/i3-and-kde-plasma) and [this](https://maxnatt.gitlab.io/posts/kde-plasma-with-i3wm/#kde-525-and-newer) but with more details and updated for Plasma 6.

## Why you might want to do this
Like a lot of people, I had an evening of panic when my [Bismuth](https://github.com/Bismuth-Forge/bismuth) install broke upon installing Plasma 6. After trying a few things, I decided I liked the convenience of KDE's integrated DE but couldn't give up tiling windows. So I followed a few guides and tried things until I landed on a set of configs with reasonable jank and good functionality. If you like:
- KDE's ease of use 
- Tiling functionality KWin scripts can't match
- A highly configurable workflow

Then this might be for you.

## Why you might not want to do this
There are a few things to keep in mind:
- This is X11-only. AFAIK Sway is incompatible with Plasma since Wayland WMs must also be compositors.
- This probably isn't going to work forever. I'm considering it a stopgap until a better KWin tiling experience happens.
- Holy hell is it janky. There's issues with popups going in the wrong places, things being transparent that shouldn't be, and lots more. Be prepared for a less flexible setup.

## The Guide
### Installation
I'm assuming you already have Plasma. We're going to be installing i3, feh for a desktop background, and picom for compositing.
```
sudo pacman -Syu i3 feh picom
```

### Configuration

### Notable Issues
- Plasma popups like the volume slider are in the wrong place.
- Some plasmoids are transparent when they needn't be (e.g. the WiFi menu).
- Pressing Meta doesn't summon the Start menu. I just use krunner for everything anyway.

These are all probably fixable via config file changes- submit a PR! I'm calling my setup supergoodenough but input is welcome.
