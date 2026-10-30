# Nightfeed — Plymouth Boot Splash

Night-vision VHS boot splash: the cobalt face under scanlines and grain, a rolling tracking band, VCR OSD, tape-block progress.

![boot](screenshots/boot.jpg)

Nightfeed is a night-vision VHS look for KDE Plasma 6, built around a cobalt-lit face on near-black: cobalt-black surfaces, faint scanlines and tape grain, and a slight violet glow on whatever has focus.

## Features

- Live grain, a tracking band rolling top to bottom, and an occasional tape wobble of the picture.
- VCR OSD: `PLAY ▶` blinks while the deck engages, plus `CH 03 SP` and a tape counter that ticks every second.
- Boot progress as a strip of 32 violet tape blocks under a glowing **NIGHTFEED**.
- Shutdown shows `STOP ■` / **EJECTING TAPE**, reboot shows `REW ◀◀`.
- Disk-unlock prompt (LUKS): a glowing field with block bullets.
- Every word is pre-rendered, so no fonts are needed in the initramfs. Laid out for 16:9 and scaled by screen height.

![password](screenshots/password.jpg)
![shutdown](screenshots/shutdown.jpg)

## Requirements

Plymouth with the `script` plugin (standard).

## Install

```bash
git clone https://github.com/numbpill3d/nightfeed-plymouth
cd nightfeed-plymouth && sudo ./install.sh
```

Or from the KDE Store: Extract to `/usr/share/plymouth/themes/`, then `sudo plymouth-set-default-theme -R nightfeed` (on dracut systems: `sudo plymouth-set-default-theme nightfeed && sudo dracut -f`).

## Configuration

Make sure `splash` is on the kernel command line.

## The rest of the suite

| piece | repo |
|---|---|
| SDDM login | [nightfeed-sddm](https://github.com/numbpill3d/nightfeed-sddm) |
| Global theme + splash screen | [nightfeed-global](https://github.com/numbpill3d/nightfeed-global) |
| Plasma style (panel, popups) | [nightfeed-plasma](https://github.com/numbpill3d/nightfeed-plasma) |
| Aurorae window decoration | [nightfeed-aurorae](https://github.com/numbpill3d/nightfeed-aurorae) |
| Colour scheme | [nightfeed-colors](https://github.com/numbpill3d/nightfeed-colors) |
| Kvantum widget style | [nightfeed-kvantum](https://github.com/numbpill3d/nightfeed-kvantum) |
| Icon theme | [nightfeed-icons](https://github.com/numbpill3d/nightfeed-icons) |
| Konsole + kitty colours | [nightfeed-konsole](https://github.com/numbpill3d/nightfeed-konsole) |

Everything at once, with the generators: [nightfeed](https://github.com/numbpill3d/nightfeed).

## Tags

`nightfeed` `kde` `plasma6` `dark` `vhs` `scanlines` `cobalt` `violet` `purple` `retro` `analog-horror` `glow` `plymouth` `plymouth-theme` `boot-splash` `bootscreen` `luks`

## Credits and licence

By splicer scorn (voidrane). GPL-3.0-or-later.
