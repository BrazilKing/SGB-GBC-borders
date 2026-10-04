# Gen1Recomp - Visual Frames & Overlays

A visual frame/overlay configuration for Gen1Recomp that supports Game Boy,
Game Boy Color, Game Boy Advance, Super Game Boy, themed Pokemon overlays,
party overlays, gym badges, day/night variants, and GB/GBC icons.

This README is based on the current `main.lua` configuration supplied with
this project.

---

## Features

The current configuration provides:

- Game Boy frame selection
- Game Boy Color frame selection
- Game Boy Advance frame selection
- Game Boy Advance SP frame selection
- Super Game Boy frame selection
- Super Game Boy Gold 97 frame selection
- Day/night frame selection
- Automatic day/night mode
- GB/GBC Pokeball icon
- GB/GBC Pokemon logo icon
- Gen 1/2 Pokemon-themed frames
- Gen 1/2 party frames
- Gen 1/2 gym badge overlays
- Gen 2 Johto gym badge support
- Gen 2 Kanto gym badge support
- Gen 3 themed frames
- Automatic gym/city badge selection
- Per-playthrough option storage
- Fallback handling when an overlay asset is unavailable
- Runtime compatibility checks between game generation and console/theme

---

# Menu Configuration

The mod currently exposes 8 menu sections.

## 1. CONSOLE

Available choices:

- NONE
- GB
- GB DARK
- GB LIGHT
- GB POCKET
- GBC
- GBA
- GBA SP
- SGB
- SGB GOLD 97

Internal values:

```text
none
gb
gb_dark
gblight
gbpocket
gbc
gba
gba_sp
sgb
sgb_gold97
```

---

## 2. DAY/NIGHT GB/SGB/GBA

Available choices:

- AUTO
- DAY
- NIGHT

Internal values:

```text
auto
day
night
```

### AUTO

AUTO determines the period from the system time.

The current implementation treats:

```text
06:00 - 17:59 = DAY
18:00 - 05:59 = NIGHT
```

The selected period is cached by minute.

### DAY

Forces the day variant.

### NIGHT

Forces the night variant.

---

# 3. POKEBALL GB/GBC

Available choices:

- OFF
- ON

Internal values:

```text
off
on
```

The icon resolver only enables this option for:

- GB
- GB DARK
- GB LIGHT
- GB POCKET
- GBC

---

# 4. PKMN LOGO GB/GBC

Available choices:

- OFF
- ON

Internal values:

```text
off
on
```

Like the Pokeball option, the Pokemon logo is only enabled by the icon
resolver for:

- GB
- GB DARK
- GB LIGHT
- GB POCKET
- GBC

---

# 5. PKMN GEN1-2

Available choices:

- NONE
- CHIKORITA
- GEODUDE
- KANGASKHAN
- MEOWTH
- NIDOKING
- PIKACHU
- TOTODILE

Internal values:

```text
none
chikorita
geodude
kangaskhan
meowth
nidoking
pikachu
totodile
```

These are Gen 1/2 themed overlays.

Supported console variants in the current themed asset table include:

- SGB
- GB
- GB DARK
- GB LIGHT
- GB POCKET
- GBC

---

# 6. PARTY GEN1-2

Available choices:

- NONE
- BLOODDLL
- DARTHTRON64
- FERNANDO
- FERNANDO B
- FOXEGORY5
- THEEON
- TORCHICISLAND
- TORCHICISLAND B
- ZEAK6464

Internal values:

```text
none
blooddll
darthtron64
fernando
fernando_b
foxegory5
theeon
torchicisland
torchicisland_b
zeak6464
```

Party variants are currently defined for:

- GB
- GB DARK
- GB LIGHT
- GB POCKET
- GBC

Party overlays have priority over the Gen 1/2 Pokemon-themed overlay.

If a requested party asset does not exist for the selected console, the mod
falls back to the base console frame when that frame is available.

---

# 7. GYM BADGE GEN 1-2

Available choices:

- NONE
- AUTO (GYM)
- AUTO (CITY)
- BOULDER
- CASCADE
- THUNDER
- RAINBOW
- SOUL
- MARSH
- VOLCANO
- EARTH

Internal values:

```text
none
auto_gym
auto_city
boulder
cascade
thunder
rainbow
soul
marsh
volcano
earth
```

Gym badge overlays are disabled for:

- SGB
- SGB GOLD 97
- GBA
- GBA SP

---

## Gen 1 / RBY Gym Mapping

| Gym | Map |
|---|---|
| Boulder | PEWTER_GYM |
| Cascade | CERULEAN_GYM |
| Thunder | VERMILION_GYM |
| Rainbow | CELADON_GYM |
| Soul | FUCHSIA_GYM |
| Marsh | SAFFRON_GYM |
| Volcano | CINNABAR_GYM |
| Earth | VIRIDIAN_GYM |

## Gen 1 / RBY City Mapping

| Badge | City |
|---|---|
| Boulder | PEWTER_CITY |
| Cascade | CERULEAN_CITY |
| Thunder | VERMILION_CITY |
| Rainbow | CELADON_CITY |
| Soul | FUCHSIA_CITY |
| Marsh | SAFFRON_CITY |
| Volcano | CINNABAR_ISLAND |
| Earth | VIRIDIAN_CITY |

### AUTO (GYM)

Selects the badge based on the current gym map.

### AUTO (CITY)

Selects the badge based on the current gym/city map.

---

# Gen 2 / GSC Gym Support

The current code also contains a separate Gen 2 badge table.

## Johto

| Badge | Map |
|---|---|
| Zephyr | VIOLET_GYM / VIOLET_CITY |
| Hive | AZALEA_GYM / AZALEA_TOWN |
| Plain | GOLDENROD_GYM / GOLDENROD_CITY |
| Fog | ECRUTEAK_GYM / ECRUTEAK_CITY |
| Storm | CIANWOOD_GYM / CIANWOOD_CITY |
| Mineral | OLIVINE_GYM / OLIVINE_CITY |
| Glacier | MAHOGANY_GYM / MAHOGANY_TOWN |
| Rising | BLACKTHORN_GYM / BLACKTHORN_CITY |

## Kanto in GSC

The GSC badge table also defines:

- Boulder
- Cascade
- Thunder
- Rainbow
- Soul
- Marsh
- Volcano
- Earth

These use GSC badge numbering 9-16.

---

# 8. PKMN GEN3

Available choices:

- NONE
- CELEBI
- SUICUNE
- POKEMON CENTER

Internal values:

```text
none
celebi
suicune
pokemoncenter
```

These are treated as Gen 3 themes.

The current themed table provides GBA and GBA SP variants for:

- Celebi
- Suicune
- Pokemon Center

---

# Game Generation Handling

The code maintains a game version from `game.ready`.

The following game versions are explicitly treated as the Game Boy/SGB
generation:

```text
red
blue
yellow
gold
silver
crystal
```

Generation 2 is detected separately for GSC badge tables:

```text
gold
silver
crystal
```

Gen 3 is detected as a non-SGB game version when a game version is available.

---

# Gen 1/2 vs Gen 3 Options

## Gen 1/2 games

The active themed selection comes from:

```text
PKMN GEN1-2
```

The active party selection comes from:

```text
PARTY GEN1-2
```

`PKMN GEN3` is not used as the active theme.

If a party overlay is selected, the party overlay takes priority over the
Gen 1/2 Pokemon theme.

## Gen 3 games

The active themed selection comes from:

```text
PKMN GEN3
```

Gen 1/2 Pokemon and party selections are not used.

The Gen 3 themed options are intended for GBA/GBA SP.

---

# Console / Game Compatibility

The resolver checks whether the selected console matches the detected game
generation.

Examples of mismatch conditions include:

```text
A Gen 1/2 console selected for a Gen 3 game
A Gen 3 console selected for a Gen 1/2 game
```

The resolver reports a warning while continuing to resolve the frame where
possible.

The code does not silently treat every menu combination as a valid unique
visual result.

---

# Overlay Priority

The current resolution order is approximately:

```text
Game generation
    |
    +-- Gen 1/2
    |     |
    |     +-- PARTY GEN1-2
    |     |
    |     +-- PKMN GEN1-2
    |
    +-- Gen 3
          |
          +-- PKMN GEN3
```

For Gen 1/2 games:

```text
PARTY GEN1-2
    >
PKMN GEN1-2
    >
Base console frame
```

For Gen 3 games:

```text
PKMN GEN3
    >
Base GBA/GBA SP frame
```

The code also performs console and theme compatibility checks before
resolving the final asset.

---

# Day/Night Resolution

The selected day/night mode affects:

- SGB default frames
- SGB Gold 97 frames
- GBA frames
- GBA SP frames
- Themed assets where a night variant is available

The implementation uses:

```text
AUTO
DAY
NIGHT
```

When AUTO is active, the local system hour is used.

For several GB/GBC themed assets, if a night-specific asset is not available,
the resolver attempts the normal/day asset before falling back to the base
frame.

---

# Asset Paths

The current `main.lua` references assets under the following general
directories:

```text
assets/
├── gb/
├── gbc/
├── gba/
├── sgb/
├── gym/
│   ├── rby/
│   └── gsc/
├── icon/
└── party/
```

---

# Base Console Frames

The current device frame table includes:

```text
assets/gb/gb/gb_4x3.png
assets/gb/gb/gb_dark_4x3.png
assets/gb/gb/gblight_4x3.png
assets/gb/gb/gbpocket_4x3.png
assets/gbc/gbc/gbc_4x3.png
assets/gba/gba/gba_4x3.png
assets/gba/gba/gba_light_4x3.png
assets/gba/gba/gba_sp_4x3.png
assets/gba/gba/gba_sp_light_4x3.png
```

SGB assets use game-specific directories and stems.

Gold 97 uses:

```text
assets/sgb/gold97/gold97_4x3.png
assets/sgb/gold97/gold97_night_4x3.png
```

---

# Icons

The current icon assets are:

```text
assets/icon/pokeball.png
assets/icon/pkmn.png
```

Both are controlled independently through the menu.

---

# Gym Badge Assets

RBY badge assets:

```text
assets/gym/rby/rby_gym_1.png
assets/gym/rby/rby_gym_2.png
assets/gym/rby/rby_gym_3.png
assets/gym/rby/rby_gym_4.png
assets/gym/rby/rby_gym_5.png
assets/gym/rby/rby_gym_6.png
assets/gym/rby/rby_gym_7.png
assets/gym/rby/rby_gym_8.png
```

GSC badge assets:

```text
assets/gym/gsc/gsc_gym_1.png
...
assets/gym/gsc/gsc_gym_16.png
```

---

# Party Asset Naming

Party assets follow the current naming scheme:

```text
assets/party/<party>/<party>_<console>_4x3.png
```

Examples:

```text
assets/party/blooddll/blooddll_gb_4x3.png
assets/party/blooddll/blooddll_gb_dark_4x3.png
assets/party/blooddll/blooddll_gblight_4x3.png
assets/party/blooddll/blooddll_gbpocket_4x3.png
assets/party/blooddll/blooddll_gbc_4x3.png
```

Variants with `B` use the corresponding `_b_` naming in the current code.

---

# Gen 1/2 Themed Asset Naming

The current code resolves themed assets using console-specific paths.

Examples:

```text
assets/gb/pikachu/pikachu_gb_4x3.png
assets/gb/pikachu/pikachu_gb_dark_4x3.png
assets/gb/pikachu/pikachu_gblight_4x3.png
assets/gb/pikachu/pikachu_gbpocket_4x3.png
assets/gbc/pikachu/pikachu_gbc_4x3.png
```

SGB assets use:

```text
assets/sgb/<pokemon>/<pokemon>_sgb_4x3.png
assets/sgb/<pokemon>/<pokemon>_night_sgb_4x3.png
```

---

# Gen 3 Themed Asset Naming

The GBA/GBA SP themed paths are resolved using the selected Pokemon theme
and console variant.

The current configuration supports:

```text
Celebi
Suicune
Pokemon Center
```

for:

```text
GBA
GBA SP
```

with day/night-aware GBA variants where applicable.

---

# Fallback Behavior

The mod checks whether requested assets exist before using them.

If a requested party or Pokemon theme cannot be found, the resolver attempts
to use the selected console's base frame.

Examples of warning situations include:

```text
No <theme> overlay for <console>.
Party frame <party> has no variant for <console>.
The <console> frame file is missing from the install.
No console selected.
```

This prevents an unavailable themed asset from automatically becoming the
only rendering result.

---

# Option Storage

The mod stores options per playthrough.

Storage keys are separated into a Game Boy/Gen 1-2 bucket and a GBA/Gen 3
bucket.

The bucket selection is:

```text
_gb
_gba
```

This allows the option values to be stored separately depending on the
detected game generation.

The default values are:

```text
console        = none
pokemon_gen12  = none
party_gen12    = none
gym_badge_gen1 = auto_gym
pokemon_gen3   = none
day_night_mode = auto
icon_pokeball  = off
icon_pkmn      = off
```

---

# Map Detection

The current map event stores the active map ID:

```text
map.entered
```

The gym badge resolver uses that map ID for automatic badge selection.

Supported RBY gym/city maps are defined directly in `main.lua`.

Supported GSC Johto gym/city maps are also defined directly in `main.lua`.

---

# Raw Configuration Count

The current menu contains:

```text
CONSOLE          = 10
DAY/NIGHT        = 3
POKEBALL         = 2
PKMN LOGO        = 2
PKMN GEN1-2      = 8
PARTY GEN1-2     = 10
GYM BADGE        = 11
PKMN GEN3        = 4
```

The raw configuration space is therefore:

```text
10 x 3 x 2 x 2 x 8 x 10 x 11 x 4
= 422,400
```

## Important

`422,400` is the number of possible menu configurations.

It is NOT the number of unique rendered overlays.

The actual number of unique visual results is lower and context-dependent
because the runtime applies:

- game-generation restrictions
- console restrictions
- overlay priority
- day/night selection
- map-based badge selection
- automatic gym/city selection
- unavailable-asset fallback
- Gen 1/2 versus Gen 3 theme handling

Therefore, a single exact number of unique rendered images cannot be
derived from the menu counts alone.

---

# Configuration Examples

## Standard Game Boy

```text
CONSOLE: GB
DAY/NIGHT: AUTO
POKEBALL: OFF
PKMN LOGO: OFF
PKMN GEN1-2: NONE
PARTY GEN1-2: NONE
GYM BADGE: AUTO (GYM)
PKMN GEN3: NONE
```

Result:

```text
Base GB frame
+
Automatic badge when supported by the current map
```

---

## GB + Pokemon Theme

```text
CONSOLE: GB
PKMN GEN1-2: PIKACHU
PARTY GEN1-2: NONE
```

The resolver attempts to use:

```text
assets/gb/pikachu/pikachu_gb_4x3.png
```

---

## GB + Party

```text
CONSOLE: GB
PKMN GEN1-2: PIKACHU
PARTY GEN1-2: BLOODDLL
```

The party overlay has priority over the Gen 1/2 Pokemon theme.

The resolver attempts to use the Blooddll GB party asset.

---

## GBC + Icons

```text
CONSOLE: GBC
POKEBALL: ON
PKMN LOGO: ON
```

Both GB/GBC icon assets are enabled by the icon resolver.

---

## GBA + Gen 3 Theme

```text
CONSOLE: GBA
PKMN GEN3: CELEBI
```

The resolver attempts to use the GBA Celebi theme.

---

## Automatic Gym Badge

```text
GYM BADGE: AUTO (GYM)
```

When entering a supported gym map, the corresponding badge is selected
automatically.

---

# Current Limitations / Important Notes

The following behavior is determined directly by the current `main.lua`:

1. The raw 422,400 count should not be described as 422,400 unique visual
   images.

2. Party overlays are Gen 1/2 content and are not used as Gen 3 themes.

3. Gen 3 Pokemon themes are separated from Gen 1/2 Pokemon themes.

4. Gym badges are not resolved for SGB, SGB Gold 97, GBA, or GBA SP.

5. GB/GBC icons are restricted to the consoles in `ICON_ALLOWED_CONSOLES`.

6. Automatic gym/city badges depend on the current map ID.

7. Automatic day/night selection depends on the system clock.

8. Missing assets can cause fallback to a base console frame or produce a
   warning.

9. Selecting `NONE` for the console means the resolver does not select a
   base frame. A selected party/theme without a console can therefore
   produce a warning instead of a rendered frame.

10. The exact set of available visual combinations depends on which asset
    files are actually present in the installed mod.

---

# Development

The main configuration and resolution logic is contained in:

```text
main.lua
```

Major sections of the file include:

```text
Option definitions
Game-version detection
Per-playthrough storage
Gym/badge data
Icon data
Day/night detection
Party overlay data
Pokemon themed overlay data
Console frame data
Path resolution
Cached resolution
```

When adding a new overlay, update the appropriate option list and the
corresponding asset-resolution table/path logic.

---

# Adding a New Party Overlay

A party overlay requires:

1. A new choice in `PARTY GEN1-2`.
2. A matching entry in `PARTY_MAP`.
3. The required console-specific PNG files.
4. Correct asset paths.

The current party system expects variants for the supported GB/GBC console
types where available.

---

# Adding a New Pokemon Theme

A Gen 1/2 theme requires:

1. A new choice in `PKMN GEN1-2`.
2. The appropriate entry in the `THEMED` table.
3. Matching files in the expected `assets/gb`, `assets/gbc`, or `assets/sgb`
   location.

A Gen 3 theme requires:

1. A new choice in `PKMN GEN3`.
2. A Gen 3 theme name in `GEN3_THEMED_NAMES`.
3. The corresponding entries in `THEMED`.
4. The required GBA/GBA SP assets.

---

# Adding a New Gym Badge

For RBY:

1. Add the badge path to `BADGE_FILES`.
2. Add the gym map to `GYM_BY_MAP` if automatic gym selection is required.
3. Add the city map to `CITY_BY_MAP` if automatic city selection is required.

For GSC:

1. Add the badge path to `BADGE_FILES_GSC`.
2. Add the gym map to `GYM_BY_MAP_GSC`.
3. Add the city map to `CITY_BY_MAP_GSC`.

---

# Repository Asset Structure

A simplified representation of the paths currently referenced by the Lua
configuration is:

```text
assets/
├── gb/
│   ├── gb/
│   └── <gen1-2-pokemon>/
├── gbc/
│   ├── gbc/
│   └── <gen1-2-pokemon>/
├── gba/
│   ├── gba/
│   └── <gen3-pokemon>/
├── gym/
│   ├── rby/
│   └── gsc/
├── icon/
│   ├── pokeball.png
│   └── pkmn.png
├── party/
│   ├── blooddll/
│   ├── darthtron64/
│   ├── fernando/
│   ├── foxegory5/
│   ├── theeon/
│   ├── torchicisland/
│   └── zeak6464/
└── sgb/
    ├── red/
    ├── blue/
    ├── yellow/
    ├── gold/
    ├── silver/
    ├── crystal/
    └── gold97/
```

This is a representation of paths referenced by `main.lua`; it does not
claim that every possible directory/file above is currently present in the
repository.

---

# Summary

Current `main.lua` provides:

```text
10 console choices
3 day/night choices
2 Pokeball choices
2 Pokemon logo choices
8 Gen 1/2 Pokemon choices
10 Gen 1/2 party choices
11 Gen 1/2 gym badge choices
4 Gen 3 Pokemon choices
```

Total raw menu combinations:

```text
422,400
```

The system then reduces those configurations through runtime rules such as
game generation, console compatibility, overlay priority, map detection,
day/night selection, and asset availability.

The result is a flexible frame/overlay system rather than 422,400 distinct
static images.

---

## License

No license information is defined by the supplied `main.lua`.

Add the project's intended license here when one has been selected for the
repository.

---

## Credits

Overlay/party names currently represented by the configuration include:

```text
Blooddll
Darthtron64
Fernando
Fernando B
Foxegory5
Theeon
Torchicisland
Torchicisland B
Zeak6464
```

Pokemon themes currently represented include:

```text
Chikorita
Geodude
Kangaskhan
Meowth
Nidoking
Pikachu
Totodile
Celebi
Suicune
Pokemon Center
```

Gym badge themes currently represented include:

```text
Boulder
Cascade
Thunder
Rainbow
Soul
Marsh
Volcano
Earth
Zephyr
Hive
Plain
Fog
Storm
Mineral
Glacier
Rising
```

