**3,887 unique possible on-screen combinations from 158 hand-drawn PNG files — no AI art.**

Manually reworked GB, GBC, GBA, and SGB overlays for Gen 1, 2, and 3 in
gen1recomp. Per-game selections, auto and selectable day/night versions,
themed Pokémon frames, party overlays, gym badges, Pokéball icons, and
Pokémon logo icons.

## What it does

The overlay draws on top of the game and is unaffected by shaders, so colors
stay crisp regardless of what filter you have enabled. Overlay changes apply
live from the mod manager — no restart needed. This version is built for
4:3 displays and is optimized specifically for the TrimUI Brick. The user has
full control over the overlay: any console and theme combination is
selectable on any supported game.

The mod also supports an optional **gym badge layer**, drawn on top of the
active frame, plus four optional **icon layers** — a Pokéball and a Pokémon
logo for GB/GBC, and a Pokéball and Pokémon logo for GBA. Its frame-selection
logic is fully cached so it does no per-frame filesystem work. Options save
per save file, so each playthrough can have its own setup.

The mod manager shows ten rows, labeled by generation so it's clear which
apply where. All rows are visible on every boot — the platform defines a
mod's options once at load and doesn't support per-game filtering. The mod
resolves whichever rows match the running game and ignores the rest.

## Frames included

- **Per-game SGB borders** for Red, Blue, Yellow, Gold, Silver, and Crystal
- **Day and night variants** for all six supported Gen 1/2 games, switchable
  manually or automatically
- **GOLD 97** — the SGB border from the Spaceworld '97 demo, with a night
  version featuring Pikablu. Selectable via the `SGB GOLD 97` console option.
- **Themed SGB frames** — CHIKORITA, GEODUDE, KANGASKHAN, MEOWTH, NIDOKING,
  PIKACHU, and TOTODILE, each with day and night variants
- **GB and GBC device frames** — plain GB, GB Light, GB Pocket, and GBC,
  plus themed variants for every Pokémon across all GB models and GBC. The
  standard Game Boy frame has both day and night art.
- **GBA device frames** — plain GBA and GBA SP, each with day and night
  variants selected through the DAY/NIGHT row
- **Themed GBA frames** — CELEBI, SUICUNE, and POKEMON CENTER, each with
  day and night variants across both GBA and GBA SP
- **PARTY overlays** — nine community-requested frames, each based on a
  contributor's current or favourite Gen 1/2 Pokémon. Available in GB,
  GB Dark, GB Light, GB Pocket, and GBC variants.
- **Sixteen gym badges** — the eight R/B/Y Kanto badges (Boulder, Cascade,
  Thunder, Rainbow, Soul, Marsh, Volcano, Earth) and the sixteen Gen 2
  badge arts from Gold/Silver/Crystal (the eight Johto badges — Zephyr,
  Hive, Plain, Fog, Storm, Mineral, Glacier, Rising — plus the eight Kanto
  badges as they appear in the GSC badge case). Drawn as a badge layer on
  top of GB and GBC frames.
- **Four icon overlays** — a Pokéball and Pokémon logo for GB/GBC frames,
  plus a Pokéball (top-left or centered) and Pokémon logo for GBA frames.
  Each is toggled independently.

## Overlay combinations

The mod ships **152 PNG files**. From them it can produce **3,887 unique
possible on-screen overlays**, and the user never has to scroll through a
flat list to reach any of them. Everything is built from ten short option
rows — CONSOLE, DAY/NIGHT, POKEBALL GB/GBC, POKEBALL GBA, PKMN LOGO GB/GBC,
PKMN LOGO GBA, PKMN GEN1-2, PKMN GEN3, PARTY GEN1-2, and GYM BADGE GEN 1-2 —
each with a handful of choices. The combinations emerge from those rows.

The mod also detects which game you are playing automatically. When
`CONSOLE = SGB` and no themed overlay is set, the correct official SGB
overlay for your game — Red, Blue, Yellow, Gold, Silver, or Crystal — is
loaded on its own, with no extra selection needed. Six official SGB
frames, each with a day and night variant, are picked for you.

The count breaks down like this:

- **GB** — 34 base/theme/party images × 11 badge states × 4 icon states = **1,496**
- **GB LIGHT** — 17 base/theme/party results × 11 badge states × 4 icon states = **748**
- **GB POCKET** — 17 base/theme/party results × 11 badge states × 4 icon states = **748**
- **GBC** — 17 base/theme/party results × 11 badge states × 4 icon states = **748**
- **SGB** — 16 base/theme results = **16**
- **SGB GOLD 97** — 1 base result × 2 day/night = **2**
- **GBA** — 4 base/theme results × 2 day/night × 8 icon states = **64**
- **GBA SP** — 4 base/theme results × 2 day/night × 8 icon states = **64**
- **Blank state** (`CONSOLE = NONE`) — **1**
- **Total on-screen overlays** — 1,496 + 748 + 748 + 748 + 16 + 2 + 64 + 64 + 1 = **3,887**

## Options

All options are in the mod manager. Rows are labeled by generation so it's
clear which apply where.

| Option | Value | What it does |
|---|---|---|
| **CONSOLE** | `NONE` | No console selected — overlay does not draw unless a theme or party is also set |
| | `GB` | Game Boy device frame (day and night variants via the DAY/NIGHT row) |
| | `SGB` | Super Game Boy. Automatically chooses the running game's SGB frame. Day/night can be changed manually. |
| | `SGB GOLD 97` | Forces the Spaceworld '97 Gold demo frame. |
| | `GB POCKET` | Game Boy Pocket device frame |
| | `GB LIGHT` | Game Boy Light device frame |
| | `GBC` | Game Boy Color device frame |
| | `GBA` | Game Boy Advance device frame (day/night via the DAY/NIGHT row) |
| | `GBA SP` | Game Boy Advance SP device frame (day/night via the DAY/NIGHT row) |
| **DAY/NIGHT GB/SGB/GBA** | `AUTO` | Picks day or night from your system clock (6am–6pm is day). Applies to SGB, GB, and GBA frames. |
| | `DAY` | Always the day variant. |
| | `NIGHT` | Always the night variant. |
| **POKEBALL GB/GBC** | `OFF` | No Pokéball icon on GB/GBC frames |
| | `ON` | Draws the Pokéball icon on top of GB and GBC frames |
| **POKEBALL GBA** | `OFF` | No Pokéball icon on GBA frames |
| | `TOP-LEFT` | Draws the Pokéball in the top-left corner |
| | `CENTER` | Draws the Pokéball centered on the frame |
| | `BOTH` | Draws both the top-left and centered Pokéballs |
| **PKMN LOGO GB/GBC** | `OFF` | No Pokémon logo icon on GB/GBC frames |
| | `ON` | Draws the Pokémon logo icon on top of GB and GBC frames |
| **PKMN LOGO GBA** | `OFF` | No Pokémon logo icon on GBA frames |
| | `ON` | Draws the Pokémon logo icon on top of GBA and GBA SP frames |
| **PKMN GEN1-2** | `NONE` | No Pokémon theme for Gen 1/2 games |
| | `CHIKORITA` / `GEODUDE` / `KANGASKHAN` / `MEOWTH` / `NIDOKING` / `PIKACHU` / `TOTODILE` | Pokémon-themed overlays for GB, GBC, and SGB. All themes have a variant for every Gen 1/2 console. |
| **PKMN GEN3** | `NONE` | No theme for Gen 3 games |
| | `CELEBI` / `SUICUNE` | Pokémon-themed overlays for GBA and GBA SP |
| | `POKEMON CENTER` | Pokémon Center themed overlay for GBA and GBA SP |
| **PARTY GEN1-2** | `NONE` | No party overlay |
| | `BLOODDLL` / `DARTHTRON64` / `FERNANDO` / `FERNANDO B` / `FOXEGORY5` / `THEEON` / `TORCHICISLAND` / `TORCHICISLAND B` / `ZEAK6464` | Community-requested party overlays. Combines with `CONSOLE` to pick the hardware variant. Gen 1/2 only. |
| **GYM BADGE GEN 1-2** | `NONE` | No badge layer |
| | `AUTO (GYM)` | Shows the matching badge when inside its gym. On Gen 1 it uses the R/B/Y badge art; on Gen 2 it uses the correct Gold/Silver/Crystal art, covering all sixteen Johto and Kanto gyms. |
| | `AUTO (CITY)` | Shows the matching badge anywhere in the corresponding city, and inside the gym |
| | `BOULDER` / `CASCADE` / `THUNDER` / `RAINBOW` / `SOUL` / `MARSH` / `VOLCANO` / `EARTH` | Forces a specific badge regardless of map |

`CONSOLE`, `POKEBALL GB/GBC`, `POKEBALL GBA`, `PKMN LOGO GB/GBC`,
`PKMN LOGO GBA`, `PKMN GEN1-2`, `PKMN GEN3`, `PARTY GEN1-2`, and
`GYM BADGE GEN 1-2` all default to `NONE`/`OFF`. If a theme is set
without `CONSOLE`, a notice appears and no overlay is drawn.

**`CONSOLE` and `PARTY` combine.** To draw a party frame, set both rows —
the console selects the hardware variant, the party row selects the
contributor. If `CONSOLE` is `NONE`, `SGB`, or `SGB GOLD 97` while a party
is set, a notice appears and the base console frame draws instead.

**`PARTY` overrides `PKMN`.** If both a party and a Pokémon theme are set,
the party frame wins.

**Icons stack on the frame.** All four icon rows draw their full-screen
overlays on top of whatever base frame, theme, party, or badge is active.
GB/GBC icons only draw on GB-family consoles. GBA icons only draw on GBA
and GBA SP. Both GBA Pokéball positions can be drawn at once via `BOTH`.
All icons are suppressed on `CONSOLE = NONE`.

## Saving per save file

Options save **per save file**, not globally. A fresh save starts at the
mod's default settings (no console, no theme, no party, no icons,
`AUTO (GYM)` badge, `AUTO` day/night). The first time you change an option
in that save, the mod writes the value into that save's storage — and only
that save.

Gen 1/2 and Gen 3 saves hold separate settings. A frame chosen while
playing Red never shows up on a FireRed boot, and vice versa.

So:

- **Red save 1** can show a GB Light frame while **Red save 2** shows an SGB
  frame.
- **Red** and **Crystal** share one bucket of GB/GBC/SGB selections.
- **Gen 3** saves have their own GBA selections, independent of any
  Gen 1/2 save.
- Starting a new game gives you the mod's defaults, not whatever you had
  selected last time.

## Generation handling

The mod resolves the generation-specific rows that apply to the running game
and ignores the rest:

- **Gen 1/2 games** (Red, Blue, Yellow, Gold, Silver, Crystal) read
  `PKMN GEN1-2`, `PARTY GEN1-2`, and `GYM BADGE GEN 1-2`. The `PKMN GEN3`
  row is ignored.
- **Gen 3 games** read `PKMN GEN3`. The `PKMN GEN1-2`, `PARTY GEN1-2`, and
  `GYM BADGE GEN 1-2` rows are ignored.

`CONSOLE`, `DAY/NIGHT`, and all four icon rows apply on both, with each
icon row restricted to its target console family by design.

The mod does not block any selection based on the running generation. When a
console or theme from the other generation's set is selected, the mod draws
the plain console frame with an informational notice rather than nothing, so
a mismatched selection never leaves the screen bare.

## GBA on Gen 1/2 games

Selecting a GBA console on a Gen 1/2 game draws the GBA frame with an
informational notice that GBA was not the hardware those games ran on. The
frame renders; the notice is informational.

Selecting a Gen 3 theme (`CELEBI`, `SUICUNE`, `POKEMON CENTER`) on a Gen 1/2
game suppresses the themed overlay — there is no Gen 1/2 art for those
themes — and draws the plain console frame with a notice.

## Gen 3 games

On Gen 3 games, GBA consoles and the Gen 3 themes (CELEBI, SUICUNE, POKEMON
CENTER) draw normally. Selecting a GB, GBC, or SGB console draws the plain
console frame with a notice, since there are no themed or party overlays for
those consoles in the Gen 3 frame set. Selecting a Gen 1/2 theme (CHIKORITA,
GEODUDE, etc.) suppresses the themed overlay and draws the plain console
frame with a notice — those themes have no Gen 3 variants. Party frames and
GB/GBC icons do not render on Gen 3.

## Gym badges

The badge is a second overlay drawn on top of the base frame, not a
replacement for it. Whatever the base overlay is — a themed GB or GBC frame,
a party overlay, or a plain GB or GBC device frame — the badge draws over
it. Every existing option keeps working exactly as before.

**SGB and GBA frames are the exceptions.** When the base overlay is a Super
Game Boy frame or a GBA frame, the badge layer is skipped entirely. SGB
frames fill the whole window with their own decorative art, and the badge
art is R/B/Y Gen 1 content that doesn't belong on a GBA frame. Badges render
only over GB and GBC variants.

Layer order:

1. Base frame — chosen by the `CONSOLE`, `PKMN`, and `PARTY` rows
2. GB/GBC icons — drawn on top when enabled and the console is GB-family
3. GBA icons — drawn on top when enabled and the console is GBA or GBA SP
4. Gym badge — drawn on top, when the badge option applies and the base
   frame is GB or GBC

**`AUTO (GYM)`** reads the current map. When the player enters a gym, the
matching badge appears. When the player leaves, it disappears. On Gen 2
games the mapping follows the Johto gym order and then the Kanto gym order,
and each badge uses the correct Gold/Silver/Crystal artwork. All sixteen
gyms are covered, including Clair's gym and Blaine's relocated gym on the
Seafoam Islands.

**`AUTO (CITY)`** extends the automatic behavior to the whole city instead
of just the gym interior. Entering Pewter City shows the Boulder Badge and
it stays visible anywhere in Pewter until the player leaves. Gym interiors
are still covered by the same badge.

Note that Viridian City is reachable at the very start of the game, before
the player has earned any badges. Selecting `AUTO (CITY)` will show the
Earth Badge on that first visit.

**Manual mode** — selecting any specific badge forces it to draw regardless
of which map the player is on.

Some combinations:

- `PARTY GEN1-2 = MEOWTH` + `GYM BADGE GEN 1-2 = AUTO (GYM)` — Meowth's
  party frame shows normally, and the Pewter badge appears when the player
  enters Pewter Gym.
- `CONSOLE = GBC` + `PKMN GEN1-2 = CHIKORITA` + `GYM BADGE GEN 1-2 = EARTH`
  — Chikorita's GBC frame is always accompanied by the Earth Badge.
- `CONSOLE = GB LIGHT` + `GYM BADGE GEN 1-2 = NONE` — clean GB Light device
  frame with no badge at all.
- `CONSOLE = SGB` + `GYM BADGE GEN 1-2 = AUTO (CITY)` — SGB frame draws
  with no badge, even inside a gym or city.
- `CONSOLE = GBA SP` + `GYM BADGE GEN 1-2 = AUTO (CITY)` — GBA SP frame
  draws with no badge, regardless of map.
- `CONSOLE = GBC` + `POKEBALL GB/GBC = ON` + `PKMN LOGO GB/GBC = ON` —
  GBC frame with both GB/GBC icons stacked on top.
- `CONSOLE = GBA` + `POKEBALL GBA = BOTH` + `PKMN LOGO GBA = ON` —
  GBA frame with both Pokéballs and the Pokémon logo stacked on top.

## Performance

- **Cached path resolution.** The mod no longer re-evaluates the full
  frame-selection tree on every frame. Previously each frame checked options,
  built asset paths, and probed the filesystem to confirm each candidate
  file existed — up to six file existence checks per frame during normal
  play. That work is now memoized. The selection is recomputed only when
  something that affects it actually changes: an option is edited, the
  player enters a new map, or the day/night period flips. The result is
  identical; only the wasted work is gone. Each layer has its own cache
  keyed on the options that affect it.
- **Zero-cost idle rendering.** When the base frame is `NONE`, no badge
  applies, and no icons are enabled, the render hook now returns before
  touching any graphics state. No canvas save, no scissor save, no color
  save, no restore. Nothing to draw means nothing is done.
- **Correct SGB frame resolution on late game-version detection.** The game
  version is now part of the cache key and is read from the live game object
  when the platform event hasn't delivered it, so if the SGB default frame is
  resolved before the game version becomes available, the correct frame is
  picked up automatically instead of being stuck on a fallback until the
  next option change.

These changes are most noticeable on lower-power devices with a frame,
badge, or icon active during normal gameplay.

## Supported games

Red, Blue, Yellow, Gold, Silver, Crystal — plus Gen 3.

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

- **The mod platform does not support per-generation option schemas.** A
  mod's options are defined once at load and cannot be filtered, hidden, or
  swapped based on the running game. That's why all ten option rows appear
  on every boot, including the rows that don't apply to the current
  generation. The row labels are the only signal.
- `CONSOLE`, `POKEBALL GB/GBC`, `POKEBALL GBA`, `PKMN LOGO GB/GBC`,
  `PKMN LOGO GBA`, `PKMN GEN1-2`, `PKMN GEN3`, `PARTY GEN1-2`, and
  `GYM BADGE GEN 1-2` default to `NONE`/`OFF`, so the overlay is
  **disabled on first launch** to prevent the UI from being cropped on
  certain devices, which can make it difficult to navigate the settings
  menu. Set any row to a real value to enable the overlay.
- Changes apply live — no restart needed
- **Options save per save file.** A fresh save starts at the mod's defaults.
  See "Saving per save file" above.
- **Gen 1/2 and Gen 3 save separate settings.** A frame chosen while playing
  Red never shows up on a FireRed boot, and vice versa.
- **DAY/NIGHT applies to SGB, GB, and GBA frames.** For SGB, it selects the
  day or night variant of the running game's frame and the themed Pokémon
  frames. For GB, it selects between the standard and dark Game Boy art.
  For GBA, it selects between the day and night art of the chosen console.
  All GBC frames are day-only, and `PARTY` overlays are day-only.
- **Icon overlays are console-family specific.** `POKEBALL GB/GBC` and
  `PKMN LOGO GB/GBC` are suppressed on SGB, SGB GOLD 97, GBA, GBA SP, and
  `CONSOLE = NONE`. `POKEBALL GBA` and `PKMN LOGO GBA` are suppressed on
  every console except GBA and GBA SP. All icons stack on top of any
  compatible frame, theme, party, or badge.
- **Gen 2 gym badges are fully supported.** On Gold, Silver, and Crystal,
  the `GYM BADGE GEN 1-2` row resolves to the correct Gold/Silver/Crystal
  badge art for all sixteen Johto and Kanto gyms. This includes Clair's gym
  and Blaine's relocated gym on the Seafoam Islands.
- **Gold defaults to the standard Gold frame.** To use the Spaceworld '97
  demo frame, select `CONSOLE = SGB GOLD 97`.
- **`PARTY GEN1-2` combines with `CONSOLE`.** Set both to draw a party frame
  on a specific hardware variant. Setting `PARTY GEN1-2` with
  `CONSOLE = NONE`, `SGB`, or `SGB GOLD 97` shows a notice and draws the
  plain console frame.
- **`PARTY GEN1-2` wins over `PKMN GEN1-2`.** If both are set, the party
  frame draws.
- **Badges render only over GB and GBC frames.** SGB and GBA frames suppress
  the badge layer by design.
- **`PKMN GEN3` has no party equivalent.** Party overlays are Gen 1/2 only.
- **If `CONSOLE = SGB` and the running game can't be identified, no overlay
  is drawn.** A notice appears on screen for 5 seconds asking you to pick a
  style manually.
- **If a theme is set but `CONSOLE` is still `NONE`**, no overlay is drawn
  and a notice appears for 5 seconds asking you to pick a console.
- **If a frame file is missing, the mod draws the plain console frame and
  shows a notice** explaining which file is missing. Nothing silently
  substitutes a different overlay.
- **All border artwork is manually reworked by the author. No AI art was
  used.**

## Installation

1. Install the `.zip` through your mod manager, **or** copy the extracted
   folder into your mods directory.
2. Enable the mod in the launcher's MODS panel.
3. Launch any supported game. The overlay is off on first launch — the game
   screen will look normal.
4. Open the mod options, set `CONSOLE` (and optionally a theme, party, badge,
   or icon row), and the frame appears immediately.

## Updating

This mod supports in-launcher updates. The launcher's MODS panel will show an
**Update** button when a newer release is available on GitHub. The
**Versions** button lets you pick any published release — useful if you need
to roll back to v1.0.4 for 16:9 or mobile use.

## Credits

Borders and mod by BrazilKing, based on original SGB frames and GBC Pokémon
editions. PARTY overlays are community-requested, each based on a
contributor's current or favourite Gen 1/2 Pokémon.
