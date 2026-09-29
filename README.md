# SGB/GBC Classic

Manually reworked SGB and GBC borders for Gen 1 & 2 in gen1recomp. Per-game
overlays, auto and selectable day/night version, universally applicable GBC
Special Pikachu Edition.

**61 pixel-perfect overlays** — every one hand-drawn, no AI art.

## What it does

The overlay draws on top of the game and is unaffected by shaders, so colors
stay crisp regardless of what filter you have enabled. Border changes apply
live from the mod manager — no restart needed. This version is built for
4:3 displays and is optimized specifically for the TrimUI Brick. The user has
full control over the overlay: any console and Pokémon theme combination is
selectable on any supported game.

## Frames included

- **Per-game SGB borders** for Red, Blue, Yellow, Gold, Silver, and Crystal
- **Day and night variants** for all six supported games, switchable manually
  or automatically
- **GOLD 97** — the SGB border from the Spaceworld '97 demo, with a night
  version featuring Pikablu. The default for Gold, and selectable on any
  other game.
- **Themed SGB frames** — CHIKORITA, KANGASKHAN, MEOWTH, NIDOKING, PIKACHU,
  and TOTODILE, each with day and night variants
- **GB and GBC device frames** — plain GB, GB Dark, GB Light, GB Pocket, and
  GBC, plus themed variants for every Pokémon across all GB models and GBC

## Options

All options are in the mod manager.

| Option | Value | What it does |
|---|---|---|
| **CONSOLE** | `NONE` | No console selected — overlay does not draw unless a Pokémon is also set |
| | `GB` | Game Boy device frame |
| | `GB DARK` | Game Boy Dark device frame |
| | `GB LIGHT` | Game Boy Light device frame |
| | `GB POCKET` | Game Boy Pocket device frame |
| | `GBC` | Game Boy Color device frame |
| | `SGB` | Super Game Boy. Automatically chooses the running game's SGB frame. Day/night can be changed manually. |
| **POKEMON** | `NONE` | No Pokémon theme — the plain console frame is shown |
| | `CHIKORITA` / `KANGASKHAN` / `MEOWTH` / `NIDOKING` / `PIKACHU` / `TOTODILE` | Pokémon-themed overlays. All themes have a variant for every console. |
| **SGB DAY/NIGHT** | `AUTO` | Picks day or night from your system clock (6am–6pm is day). Only affects SGB frames. |
| | `DAY` | Always the day frame. |
| | `NIGHT` | Always the night frame. |

Both `CONSOLE` and `POKEMON` default to `NONE`, so the overlay does not draw
until at least one is set to a real value. If `POKEMON` is set without
`CONSOLE`, a notice appears and no overlay is drawn.

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

Running a 4:3-only release on a non-4:3 screen will stretch the artwork.

## Testing

**All 4:3 functionality has been tested and is working on the TrimUI Brick.**

**Feedback is welcome** — through GitHub issues or the gen1recomp Discord mod
section. If you report from another device, please include your device,
resolution, and how the borders rendered.

## Notes

- Both `CONSOLE` and `POKEMON` default to `NONE`, so the overlay is
  **disabled on first launch** to prevent the UI from being cropped on
  certain devices, which can make it difficult to navigate the settings
  menu. Set either row to a real value to enable the overlay.
- Changes apply live — no restart needed
- **SGB DAY/NIGHT applies to the SGB frames** — the seven game frames
  (RED through CRYSTAL, plus GOLD 97 via `AUTO`) and the six themed SGB
  frames (CHIKORITA, KANGASKHAN, MEOWTH, NIDOKING, PIKACHU, TOTODILE). All
  GBC and GB frames are day-only.
- **If `CONSOLE = SGB` and the running game can't be identified, no overlay
  is drawn.** A notice appears on screen for 5 seconds asking you to pick a
  style manually.
- **If `POKEMON` is set but `CONSOLE` is still `NONE`**, no overlay is drawn
  and a notice appears for 5 seconds asking you to pick a console.
- **Every Pokémon theme has a frame for every console**, so no fallback
  notice should appear in normal use.
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
4. Open the mod options, set `CONSOLE` (and optionally `POKEMON`), and the
   frame appears immediately.

**On gen1recomp v0.3.22 – v0.3.29:** the mod manager's update feature is
broken. See the **Updating** section for manual install instructions.

## Updating

This mod supports in-launcher updates. The launcher's MODS panel will show an
**Update** button when a newer release is available on GitHub. The
**Versions** button lets you pick any published release — useful if you need
to roll back to v1.0.4 for 16:9 or mobile use.

**Important:** gen1recomp **v0.3.22 through v0.3.29** have a broken mod
updater. If you are on any of these engine versions, the launcher's
**Update** button will fail and the mod will not install through the mod
manager.

**Install or update manually on v0.3.22 – v0.3.29:**

1. Download the `.zip` from the GitHub releases page.
2. Extract the folder.
3. Copy the extracted `sgb_gbc_borders` folder into your mods directory,
   replacing the existing one.
4. Restart the launcher.

Engine versions outside this range may have a working updater. If the
**Update** button is visible and works, use it. If it fails, fall back to
the manual steps above.

## Credits

Borders and mod by BrazilKing, based on original SGB frames and GBC Pokémon
editions.
