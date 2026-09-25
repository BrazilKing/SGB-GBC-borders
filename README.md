# SGB/GBC Classic

Manually reworked SGB and GBC borders for Gen 1 & 2 in gen1recomp. Per-game
overlays, auto and selectable day/night version, universally applicable GBC
Special Pikachu Edition. No AI art.

## What it does

The overlay draws on top of the game and is unaffected by shaders, so colors
stay crisp regardless of what filter you have enabled. Border changes apply
live from the mod manager — no restart needed. This version is built for
4:3 displays and is optimized specifically for the TrimUI Brick. The user has
full control over the overlay: any style is selectable on any supported game.

## Frames included

- **Per-game SGB borders** for Red, Blue, Yellow, Gold, Silver, and Crystal
- **Day and night variants** for all six supported games, switchable manually
  or automatically
- **GOLD 97** — the SGB border from the Spaceworld '97 demo, with a night
  version featuring Pikablu. The default for Gold, and selectable on any
  other game.
- **Additional universal frames** — GB, GB Pocket, GB Light, GBC Special
  Pikachu Edition, and NIDOKING, all usable with all six supported games

## Options

All options are in the mod manager.

| Option | Value | What it does |
|---|---|---|
| **OVERLAY** | on / off | Master switch. **Off by default** — turn on after first launch. Disabled initially so the launcher UI isn't cropped on some devices, which would make settings hard to navigate. |
| **OVERLAY STYLE** | `AUTO` | Picks the frame matching the running game. Gold defaults to GOLD 97. |
| | `RED` | Red frame — usable with all six supported games |
| | `BLUE` | Blue frame — usable with all six supported games |
| | `YELLOW` | Yellow frame — usable with all six supported games |
| | `GOLD` | Gold frame — usable with all six supported games |
| | `GOLD 97` | Spaceworld '97 demo frame — usable with all six supported games |
| | `SILVER` | Silver frame — usable with all six supported games |
| | `CRYSTAL` | Crystal frame — usable with all six supported games |
| | `GB` | Original Game Boy frame — usable with all six supported games |
| | `GB POCKET` | Game Boy Pocket frame — usable with all six supported games |
| | `GB LIGHT` | Game Boy Light frame — usable with all six supported games |
| | `GBC YELLOW` | GBC Special Pikachu Edition frame — usable with all six supported games |
| | `NIDOKING` | Nidoking frame — usable with all six supported games |
| **DAY/NIGHT MODE** | `AUTO` | Picks day or night from your system clock (6am–6pm is day). |
| | `DAY` | Always the day frame. |
| | `NIGHT` | Always the night frame. |

## Supported games

Red, Blue, Yellow, Gold, Silver, Crystal — all six supported games.

## Display

This version of the mod is **optimized for the TrimUI Brick** at 1024×768.
On that resolution every frame is pixel-perfect.

Other resolutions scale the artwork proportionally, and the result depends on
the specific device. If your screen is not 1024×768, the frames will still
display, but exact pixel alignment is not guaranteed.

All 4:3 screens have been updated to the new 4:3 viewport that ships with
gen1recomp v0.3.5 onwards.

This build represents the intended final quality level of the mod. Every
detail has been manually maximised within the author's capabilities. That
quality is specific to 1024×768; other resolutions are outside the intended
experience.

## 16:9 and mobile devices

**Support for 16:9 and mobile screens has been removed in this version.**
Automatic aspect ratio detection had a slight negative performance impact on
handhelds and offered little benefit, since their screens are already 4:3.
The process of reworking overlays for every aspect ratio and screen position
proved too complex to maintain alongside the 4:3 set.

If you are on a 16:9 or mobile device, **use v1.0.4** instead. That release
contains partial 16:9 and mobile support, though it is incomplete and was not
fully tested on those screens.

Running v1.0.8 on a non-4:3 screen will stretch the artwork.

## Testing

**All 4:3 functionality has been tested and is working on the TrimUI Brick.**

**Feedback is welcome** — through GitHub issues or the gen1recomp Discord mod
section. If you report from another device, please include your device,
resolution, and how the borders rendered.

## Notes

- The overlay is **disabled on first launch** to prevent the UI from being
  cropped on certain devices, which can make it difficult to navigate the
  settings menu. Turn on **OVERLAY** once the mod is enabled.
- Changes apply live — no restart needed
- The GB, GB Pocket, GB Light, GBC Pikachu, and NIDOKING frames have a
  single version and do not change with `DAY/NIGHT MODE`. The six game
  frames have day and night variants.
- If a frame file is missing, the mod shows an on-screen warning instead of
  drawing a fallback
- **All border artwork is manually reworked by the author. No AI art was
  used.**

## Installation

1. Install the `.zip` through your mod manager, **or** copy the extracted
   folder into your mods directory.
2. Enable the mod in the launcher's MODS panel.
3. Launch any supported game. The overlay is off on first launch — the game
   screen will look normal.
4. Open the mod options and turn on **OVERLAY**. The frame appears immediately.

## Updating

This mod supports in-launcher updates. The launcher's MODS panel will show an
**Update** button when a newer release is available on GitHub. The
**Versions** button lets you pick any published release — useful if you need
to roll back to v1.0.4 for 16:9 or mobile use.

## Credits

Borders and mod by BrazilKing, based on original SGB frames and GBC Pokémon
editions.
