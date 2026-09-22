# SGB/GBC Classic

Manually reworked SGB and GBC borders for Gen 1 & 2 in gen1recomp. Per-game
overlays, auto and selectable day/night version, universally applicable GBC
Special Pikachu Edition. No AI art.

## What it does

The overlay draws on top of the game and is unaffected by shaders, so colors
stay crisp regardless of what filter you have enabled. Border changes apply
live from the mod manager — no restart needed. The mod also detects your
screen's aspect ratio automatically and picks the closest matching frame, and
reads the launcher's screen position setting to select a matching overlay when
one exists. On a phone, this means the mod automatically follows both the
chosen screen position and the device's orientation — switching between
horizontal and vertical layouts for Pokémon Red as the device rotates.

## Frames included

- **Per-game SGB borders** for Red, Blue, Yellow, Gold, Silver, and Crystal
- **Multiple backgrounds for Red** — four aspect ratios, with position
  variants (Center / Upper / Top) for 20:9 and 9:20
- **Day and night variants** for Blue, Yellow, Gold, Silver, and Crystal,
  switchable manually or automatically
- **Universal GBC Special Pikachu Edition frame** — usable with any supported
  game
- **GOLD 97** — the SGB border from the Spaceworld '97 demo — usable with any
  supported game, for four aspect ratios

## Options

All options are in the mod manager.

| Option | Value | What it does |
|---|---|---|
| **OVERLAY** | on / off | Master switch. Off draws nothing. |
| **BACKGROUND** | `AUTO` | Picks day or night from your system clock on games that have a night frame. |
| | `DAY` | Always the day frame. |
| | `NIGHT` | Always the night frame where available. Falls back to the day frame on games that only have day art (currently Red). |
| | `GBC YELLOW` | GBC Special Pikachu Edition frame, regardless of which game is running. |
| | `GOLD 97` | The Spaceworld '97 demo border, regardless of which game is running. |
| **SCREEN ASPECT RATIO** | `AUTO (DETECT)` | Picks the closest match from the screen's current dimensions. |
| | `4:3 (HANDHELD)` | 1024×768 |
| | `16:9 NO BEZEL (SAFE)` | 1920×1080 without the blue frame |
| | `16:9 BEZEL (TEST)` | 1920×1080 with the blue frame |
| | `20:9 (LANDSCAPE)` | 2400×1080 |
| | `9:20 (PORTRAIT)` | 1080×2400 |

## Supported games

Red, Blue, Yellow, Gold, Silver, Crystal.

## Display

The border artwork is authored at 1024×768, the native resolution of the
**TrimUI Brick**. On that device every frame renders 1:1 — no scaling, no
interpolation, pixel-perfect.

The mod detects your screen's aspect ratio and picks the closest matching
frame automatically. You can override this with the **SCREEN ASPECT RATIO**
option. Aspect variants are available for Red and for the GOLD 97 frame.
Other games fall back to their 4:3 frame when a matching aspect is
unavailable.

The mod also reads the launcher's **screen position** setting (Center /
Upper / Top) and prefers a matching overlay file when one exists. Currently
only Red has position variants, and only for the 20:9 and 9:20 aspects. On
every other frame the position is ignored and the standard overlay is drawn.

## Testing

**All functionality has been 100% tested and working on the TrimUI Brick.**

**Support for other devices is not ready yet.** The mod should work on
anything that runs gen1recomp, but behavior on other screens and aspect
ratios is unverified.

**Feedback is welcome** — through GitHub issues or the gen1recomp Discord mod
section. If you report from another device, please include your device,
resolution, and how the borders rendered.

## Notes

- Changes apply live — no restart needed
- **Automatic aspect ratio selection only applies to overlays that have been
  reworked in all supported aspect ratios.** Currently that means Red and the
  GOLD 97 frame. Other overlays only have a 4:3 version and render at that
  ratio regardless of the screen.
- **Screen position variants currently only exist for Red at 20:9 and 9:20.**
  Other frames ignore the launcher's position setting.
- `16:9 BEZEL (TEST)` is experimental and needs testing
- **All border artwork is manually reworked by the author. No AI art was used.**

## Installation

1. Install the `.zip` through your mod manager, **or** copy the extracted
   folder into your mods directory.
2. Enable the mod in the launcher's MODS panel.
3. Launch any supported game.

## Updating

This mod supports in-launcher updates. The launcher's MODS panel will show an
**Update** button when a newer release is available on GitHub. The
**Versions** button lets you pick any published release if you need to roll
back.

## Credits

Borders and mod by BrazilKing, based on original SGB frames and GBC Pokémon
editions.
