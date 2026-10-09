**641,021 overlay combinations from 218 hand-drawn PNG files — no AI art.**

Manually reworked GB, GBC, GBA, SGB, and Hoenn overlays for Gen 1, 2,
FireRed, LeafGreen, Ruby, Sapphire, and Emerald in gen1recomp. Per-game
selections, auto and selectable day/night versions, themed Pokémon
frames, party overlays, gym badges, earned badges, Pokéball icons, and
Pokémon logo icons.

**What it does**

The overlay draws on top of the game and is unaffected by shaders, so
colors stay crisp regardless of what filter you have enabled. Overlay
changes apply live from the mod manager — no restart needed. This
version is built for 4:3 displays and is optimized specifically for the
TrimUI Brick. The user has full control over the overlay: any console
and theme combination is selectable on any supported game.

The mod also supports an optional gym badge layer, drawn on top of the
active frame, plus optional icon layers — a Pokéball, a Pokémon logo,
and GBA-only center/right Pokéballs with size control. All icons and the
badge are drawn full-screen on top of the active frame. Its frame-
selection logic is fully cached so it does no per-frame filesystem work.
Options save per save file, so each playthrough can have its own setup.

The mod manager shows sixteen rows, labeled so it's clear which apply
where. All rows are visible on every boot — the platform defines a mod's
options once at load and doesn't support per-game filtering. The mod
resolves whichever rows match the running game and ignores the rest.

**Frames included**

- Per-game automatic SGB borders for Red, Blue, Yellow, Gold, Silver,
  and Crystal
- Day and night variants for all six supported Gen 1/2 games, switchable
  manually or automatically
- GOLD 97 — the SGB border from the Spaceworld '97 demo, with a night
  version featuring Pikablu. Selectable via the SGB GOLD 97 console
  option.
- Themed SGB frames — CHIKORITA, GEODUDE, KANGASKHAN, MEOWTH, NIDOKING,
  PIKACHU, and TOTODILE, each with day and night variants
- GB and GBC device frames — plain GB, GB Light, GB Pocket, and GBC,
  plus themed variants for every Pokémon across all GB models and GBC.
  The standard Game Boy frame has both day and night art.
- GBA device frames — plain GBA and GBA SP, each with day and night
  variants selected through the DAY/NIGHT row
- Themed GBA frames — CELEBI, SUICUNE, and POKEMON CENTER, each with day
  and night variants across both GBA and GBA SP
- PARTY overlays — nine community-requested frames, each based on a
  contributor's current or favourite Gen 1/2 Pokémon. Available in GB,
  GB Dark, GB Light, GB Pocket, and GBC variants.
- Forty gym badges — the eight R/B/Y Kanto badges (Boulder, Cascade,
  Thunder, Rainbow, Soul, Marsh, Volcano, Earth), the sixteen Gen 2
  badge arts from Gold/Silver/Crystal (the eight Johto badges — Zephyr,
  Hive, Plain, Fog, Storm, Mineral, Glacier, Rising — plus the eight
  Kanto badges as they appear in the GSC badge case), the eight FireRed
  / LeafGreen Kanto badges, and the eight Hoenn badges from Ruby /
  Sapphire / Emerald. Drawn as a badge layer on top of GB, GBC, and GBA
  frames.
- Earned badge overlays — FireRed / LeafGreen and Ruby / Sapphire /
  Emerald. Left, top, or both placements, with AUTO modes that read the
  save file.
- Icon overlays — Pokéball (toggles on/off, console-aware), Pokémon logo
  (toggles on/off), plus GBA-only CENTER BALL GEN3 and RIGHT BALL GEN3
  toggles with a BALL SIZE GEN3 selector (SMALL / MEDIUM / LARGE / XL).

**Overlay combinations**

The mod ships 218 PNG files. From them it can produce 641,021 unique
possible on-screen overlays across all supported games.

Nothing is presented as a flat list — everything is built from sixteen
short option rows (CONSOLE, DAY/NIGHT, PARTY GEN1-2, PKMN GEN1-2,
PKMN GEN3, EARNED BADGES FRLG, EARNED BADGES RSE, GYM BADGE GEN1,
GYM BADGE GEN2, GYM BADGE FRLG, GYM BADGE RSE, PKMN LOGO, POKEBALL,
CENTER BALL GEN3, RIGHT BALL GEN3, BALL SIZE GEN3), each with a handful
of choices. The combinations emerge from those rows.

A configuration is only counted when it is valid for the running game:
mismatched console/theme picks, blocked rows, and options ignored by
that generation are excluded. Selectors (AUTO (GYM), AUTO (CITY),
LEFT AUTO, TOP AUTO, BOTH AUTO) are counted as the distinct choices they
are.

**How each console resolves**

Each rendered overlay is a stack of up to four layers:

1. Frame — device, theme, or party image (always present when a console
   is chosen)
2. Icons — Pokéball, Pokémon logo, and (GBA only) center/right Pokéballs
3. Gym badge — Gen 1/2 GB-family, or Gen 3 GBA only
4. Earned badges — Gen 3 GBA only

**Gen 1 (Red, Blue, Yellow)**

GB — 17 frame-content results (1 plain + 7 themes + 9 party) × 2
day/night × 4 icon states × 11 badge states = 1,496

GB LIGHT — 17 × 1 × 4 × 11 = 748

GB POCKET — 17 × 1 × 4 × 11 = 748

GBC — 17 × 1 × 4 × 11 = 748

SGB — (1 plain + 7 themes) × 2 day/night = 16

SGB GOLD 97 — 1 × 2 day/night = 2

Gen 1 total: 1,496 + 748 + 748 + 748 + 16 + 2 = 3,758

**Gen 2 (Gold, Silver, Crystal)**

Same structure as Gen 1, but GYM BADGE GEN2 has 19 choices (none +
AUTO (GYM) + AUTO (CITY) + 8 Johto + 8 Kanto GSC).

GB — 17 × 2 × 4 × 19 = 2,584

GB LIGHT — 17 × 1 × 4 × 19 = 1,292

GB POCKET — 17 × 1 × 4 × 19 = 1,292

GBC — 17 × 1 × 4 × 19 = 1,292

SGB — (1 + 7) × 2 = 16

SGB GOLD 97 — 1 × 2 = 2

Gen 2 total: 2,584 + 1,292 + 1,292 + 1,292 + 16 + 2 = 6,478

**Gen 3 Hoenn (Ruby, Sapphire, Emerald)**

GBA consoles only. Party frames are Gen 1/2 only.

GBA / GBA SP — 4 theme results (none + celebi + suicune + pokemoncenter)
× 2 day/night × 64 icon combos × 11 badge states × 28 earned-badge
states = 157,696 per console

Hoenn total: 157,696 + 157,696 = 315,392

**FireRed / LeafGreen**

GBA consoles only. All four layers are live.

GBA / GBA SP — 4 theme results × 2 day/night × 64 icon combos ×
11 badge states × 28 earned-badge states = 157,696 per console

FireRed/LeafGreen total: 157,696 + 157,696 = 315,392

**Blank state**

CONSOLE = NONE — no overlay drawn = 1

**Grand total**

- Red, Blue, Yellow           3,758
- Gold, Silver, Crystal       6,478
- Firered, LeafGreen          315,392
- Ruby, Sapphire, Emerald     315,392
- Blank state (CONSOLE=NONE)  1

- **Total                       641,021**

**Why 641,021 combinations produce ~296,877 distinct screens**

Some selectable choices resolve to the same rendered image:

- AUTO (GYM) and AUTO (CITY) pick one of the existing badge images
  (11 badge choices → 9 distinct images; 19 → 17 on Gen 2)
- LEFT AUTO, TOP AUTO, BOTH AUTO earned badges pick one of the forced
  counts (28 earned choices → 25 distinct earned layers)
- BALL SIZE GEN3 has no effect when RIGHT BALL GEN3 is off
  (64 icon combos → 40 distinct icon sets)

Collapsing these produces approximately 296,877 distinct composited
screens across all games. Almost the entire difference comes from the
Gen 3 games, where all three collapses stack multiplicatively:

  option states per Gen 3 console:   4 × 2 × 64 × 11 × 28 = 157,696
  distinct images per Gen 3 console: 4 × 2 × 40 ×  9 × 25 =  72,000

Four Gen 3 consoles (GBA and GBA SP, once for Hoenn and once for FRLG)
contribute 4 × 72,000 = 288,000 distinct screens. Gen 1 contributes
3,078; Gen 2 contributes 5,798; blank state is 1.

The 641,021 figure is the selectable count. The ~296,877 figure is the
visual count. Both are valid, and both exclude illegal cross-generation
states.

**Options**

All options are in the mod manager. Rows are ordered with universal
settings at the top, then generation-specific rows below.

CONSOLE
  NONE           No console selected — overlay does not draw unless a
                 theme or party is also set
  GB             Game Boy device frame (day and night variants via the
                 DAY/NIGHT row)
  SGB            Super Game Boy. Automatically chooses the running
                 game's SGB frame. Day/night can be changed manually.
  SGB GOLD 97    Forces the Spaceworld '97 Gold demo frame.
  GB POCKET      Game Boy Pocket device frame
  GB LIGHT       Game Boy Light device frame
  GBC            Game Boy Color device frame
  GBA            Game Boy Advance device frame (day/night via the
                 DAY/NIGHT row)
  GBA SP         Game Boy Advance SP device frame (day/night via the
                 DAY/NIGHT row)

DAY/NIGHT
  AUTO           Picks day or night from your system clock (6am–6pm is
                 day). Applies to SGB, GB, and GBA frames.
  DAY            Always the day variant.
  NIGHT          Always the night variant.

PARTY GEN1-2
  NONE
  BLOODDLL
  DARTHTRON64
  FERNANDO
  FERNANDO B
  FOXEGORY5
  THEEON
  TORCHICISLAND
  TORCHICISLAND B
  ZEAK6464

  Community-requested party overlays. Combines with CONSOLE to pick
  the hardware variant. Gen 1/2 only.

PKMN GEN1-2
  NONE
  CHIKORITA
  GEODUDE
  KANGASKHAN
  MEOWTH
  NIDOKING
  PIKACHU
  TOTODILE

  Pokémon-themed overlays for GB, GBC, and SGB. All themes have a
  variant for every Gen 1/2 console.

PKMN GEN3
  NONE
  CELEBI
  SUICUNE
  POKEMON CENTER

  Pokémon-themed overlays for GBA and GBA SP.

EARNED BADGES FRLG
  NONE
  LEFT AUTO
  TOP AUTO
  BOTH AUTO
  LEFT 1 – LEFT 8
  TOP 1 – TOP 8
  BOTH 1 – BOTH 8

  FireRed / LeafGreen earned badge layer. AUTO modes read the save
  file's badge flags and draw exactly the badges the player has earned
  (order-independent). Numbered modes force a specific count.

EARNED BADGES RSE
  NONE
  LEFT AUTO
  TOP AUTO
  BOTH AUTO
  LEFT 1 – LEFT 8
  TOP 1 – TOP 8
  BOTH 1 – BOTH 8

  Ruby / Sapphire / Emerald earned badge layer. Same structure as
  EARNED BADGES FRLG. AUTO modes are order-independent, so Emerald's
  out-of-order play displays correctly.

GYM BADGE GEN1
  NONE
  AUTO (GYM)     Shows the matching badge when inside its gym (Kanto
                 gym order)
  AUTO (CITY)    Shows the matching badge anywhere in the corresponding
                 Kanto city, and inside the gym
  BOULDER
  CASCADE
  THUNDER
  RAINBOW
  SOUL
  MARSH
  VOLCANO
  EARTH

  RBY badge layer. Drawn on GB and GBC consoles.

GYM BADGE GEN2
  NONE
  AUTO (GYM)     Shows the matching badge when inside its gym (Johto
                 order, then Kanto GSC order)
  AUTO (CITY)    Shows the matching badge anywhere in the corresponding
                 city, and inside the gym
  ZEPHYR
  HIVE
  PLAIN
  FOG
  STORM
  MINERAL
  GLACIER
  RISING
  BOULDER (GSC)
  CASCADE (GSC)
  THUNDER (GSC)
  RAINBOW (GSC)
  SOUL (GSC)
  MARSH (GSC)
  VOLCANO (GSC)
  EARTH (GSC)

  GSC badge layer. Drawn on GB and GBC consoles. Covers all sixteen
  Johto and Kanto gyms, including Clair's gym at BLACKTHORN_GYM_1F and
  Blaine's relocated gym at SEAFOAM_GYM.

GYM BADGE FRLG
  NONE
  AUTO (GYM)
  AUTO (CITY)
  BOULDER
  CASCADE
  THUNDER
  RAINBOW
  SOUL
  MARSH
  VOLCANO
  EARTH

  FireRed / LeafGreen Kanto badge layer. Drawn on GBA and GBA SP.

GYM BADGE RSE
  NONE
  AUTO (GYM)
  AUTO (CITY)
  STONE
  KNUCKLE
  DYNAMO
  HEAT
  BALANCE
  FEATHER
  MIND
  RAIN

  Ruby / Sapphire / Emerald Hoenn badge layer. Drawn on GBA and GBA SP.

PKMN LOGO
  OFF
  ON             Draws the Pokémon logo icon on top of GB, GBC, GBA, and
                 GBA SP frames.

POKEBALL
  OFF
  ON             Draws the Pokéball icon. On GB-family consoles this is
                 the standard GB/GBC Pokéball; on GBA / GBA SP this is
                 the top-left GBA Pokéball.

CENTER BALL GEN3
  OFF
  ON             Draws the centered GBA Pokéball. GBA and GBA SP only.

RIGHT BALL GEN3
  OFF
  ON             Draws the right-side GBA Pokéball. GBA and GBA SP only.

BALL SIZE GEN3
  SMALL          Right Pokéball drawn at small size (default)
  MEDIUM         Right Pokéball drawn at medium size
  LARGE          Right Pokéball drawn at large size
  XL             Right Pokéball drawn at extra-large size

CONSOLE, PARTY GEN1-2, PKMN GEN1-2, PKMN GEN3, EARNED BADGES FRLG,
EARNED BADGES RSE, GYM BADGE GEN1/2/FRLG/RSE, PKMN LOGO, POKEBALL,
CENTER BALL GEN3, and RIGHT BALL GEN3 all default to NONE/OFF. If a
theme is set without CONSOLE, a notice appears and no overlay is drawn.

CONSOLE and PARTY combine. To draw a party frame, set both rows — the
console selects the hardware variant, the party row selects the
contributor. If CONSOLE is NONE, SGB, or SGB GOLD 97 while a party is
set, a notice appears and the base console frame draws instead.

PARTY overrides PKMN. If both a party and a Pokémon theme are set, the
party frame wins.

Icons and badges stack on the frame. The POKEBALL, PKMN LOGO,
CENTER BALL GEN3, and RIGHT BALL GEN3 overlays draw full-screen on top
of whatever base frame, theme, party, or badge is active. The POKEBALL
row resolves to different assets depending on the current console: on
GB-family consoles it draws the standard GB/GBC Pokéball; on GBA /
GBA SP it draws the top-left GBA Pokéball. CENTER BALL GEN3 and
RIGHT BALL GEN3 draw only when the console is GBA or GBA SP, and
BALL SIZE GEN3 only affects the right-side ball. All icons are
suppressed on CONSOLE = NONE, SGB, and SGB GOLD 97.

**Saving per save file**

Options save per save file, not globally. A fresh save starts at the
mod's default settings (no console, no theme, no party, no icons,
AUTO (GYM) badge, AUTO day/night). The first time you change an option
in that save, the mod writes the value into that save's storage — and
only that save.

Gen 1/2 and Gen 3 saves hold separate settings. A frame chosen while
playing Red never shows up on a FireRed boot, and vice versa.

So:

- Red save 1 can show a GB Light frame while Red save 2 shows an SGB
  frame.
- Red and Crystal share one bucket of GB/GBC/SGB selections.
- Gen 3 saves have their own GBA selections, independent of any Gen 1/2
  save.
- Starting a new game gives you the mod's defaults, not whatever you had
  selected last time.

**Generation handling**

The mod resolves the generation-specific rows that apply to the running
game and ignores the rest:

- Gen 1/2 games (Red, Blue, Yellow, Gold, Silver, Crystal) read
  PARTY GEN1-2, PKMN GEN1-2, GYM BADGE GEN1, and GYM BADGE GEN2. The
  PKMN GEN3, EARNED BADGES FRLG/RSE, GYM BADGE FRLG/RSE rows are
  ignored.

- Gen 3 games read PKMN GEN3, EARNED BADGES FRLG or EARNED BADGES RSE
  (depending on the game), and GYM BADGE FRLG or GYM BADGE RSE. The
  PKMN GEN1-2, PARTY GEN1-2, and GYM BADGE GEN1/2 rows are ignored.

CONSOLE, DAY/NIGHT, PKMN LOGO, POKEBALL, CENTER BALL GEN3,
RIGHT BALL GEN3, and BALL SIZE GEN3 apply on all games, with the GBA-
only icon rows restricted to GBA and GBA SP consoles and the badge
layer restricted to consoles with matching art.

The mod does not block any selection based on the running generation.
When a console or theme from the other generation's set is selected,
the mod draws the plain console frame with an informational notice
rather than nothing, so a mismatched selection never leaves the screen
bare.

**GBA on Gen 1/2 games**

Selecting a GBA console on a Gen 1/2 game draws the GBA frame with an
informational notice that GBA was not the hardware those games ran on.
The frame renders; the notice is informational.

Selecting a Gen 3 theme (CELEBI, SUICUNE, POKEMON CENTER) on a Gen 1/2
game suppresses the themed overlay — there is no Gen 1/2 art for those
themes — and draws the plain console frame with a notice.

**Gen 3 games**

On Gen 3 games, GBA consoles and the Gen 3 themes (CELEBI, SUICUNE,
POKEMON CENTER) draw normally. Selecting a GB, GBC, or SGB console draws
the plain console frame with a notice, since there are no themed or
party overlays for those consoles in the Gen 3 frame set. Selecting a
Gen 1/2 theme (CHIKORITA, GEODUDE, etc.) suppresses the themed overlay
and draws the plain console frame with a notice — those themes have no
Gen 3 variants. Party frames do not render on Gen 3.

**Gym badges**

The badge is a second overlay drawn on top of the base frame, not a
replacement for it. Whatever the base overlay is — a themed GB or GBC
frame, a party overlay, or a plain device frame — the badge draws over
it. Every existing option keeps working exactly as before.

Console support for badges:

- GB and GBC family — badges draw over the frame on Gen 1 and Gen 2
  games.
- GBA and GBA SP — badges draw over the frame on FireRed, LeafGreen,
  Ruby, Sapphire, and Emerald.
- SGB and SGB GOLD 97 — badges are never drawn.

Layer order:

1. Base frame — chosen by the CONSOLE, PKMN, and PARTY rows
2. Icons — POKEBALL, PKMN LOGO, CENTER BALL GEN3, and RIGHT BALL GEN3,
   drawn on top when enabled and the console is compatible
3. Gym badge — drawn on top, when the badge option applies and the
   console supports it
4. Earned badges — drawn on top (Gen 3 GBA only)

AUTO (GYM) reads the current map. When the player enters a gym, the
matching badge appears. When the player leaves, it disappears. On Gen 1
and FireRed/LeafGreen the mapping follows the Kanto gym order. On Gen 2
it follows the Johto gym order and then the Kanto gym order, and each
badge uses the correct Gold/Silver/Crystal artwork. All sixteen Gen 2
gyms are covered, including Clair's gym at BLACKTHORN_GYM_1F and
Blaine's relocated gym at SEAFOAM_GYM. On Hoenn it follows the eight
Hoenn gyms.

AUTO (CITY) extends the automatic behavior to the whole city instead of
just the gym interior. Entering Pewter City shows the Boulder Badge and
it stays visible anywhere in Pewter until the player leaves. Gym
interiors are still covered by the same badge.

Note that Viridian City is reachable at the very start of the game,
before the player has earned any badges. Selecting AUTO (CITY) will show
the Earth Badge on that first visit.

Manual mode — selecting any specific badge forces it to draw regardless
of which map the player is on.

Some combinations:

- PARTY GEN1-2 = MEOWTH + GYM BADGE GEN1 = AUTO (GYM) — Meowth's party
  frame shows normally, and the Pewter badge appears when the player
  enters Pewter Gym.
- CONSOLE = GBC + PKMN GEN1-2 = CHIKORITA + GYM BADGE GEN1 = EARTH —
  Chikorita's GBC frame is always accompanied by the Earth Badge.
- CONSOLE = GB LIGHT + GYM BADGE GEN1 = NONE — clean GB Light device
  frame with no badge at all.
- CONSOLE = SGB + GYM BADGE GEN1 = AUTO (CITY) — SGB frame draws with
  no badge, even inside a gym or city.
- CONSOLE = GBA SP + GYM BADGE FRLG = AUTO (CITY) — GBA SP frame draws
  with no badge on non-FRLG games, and draws the matching Kanto badge on
  FireRed or LeafGreen.
- CONSOLE = GBC + POKEBALL = ON + PKMN LOGO = ON — GBC frame with both
  icons stacked on top.
- CONSOLE = GBA + POKEBALL = ON + CENTER BALL GEN3 = ON +
  RIGHT BALL GEN3 = ON + BALL SIZE GEN3 = LARGE + PKMN LOGO = ON — GBA
  frame with all four icons stacked on top.
- CONSOLE = GBA + PKMN GEN3 = CELEBI + GYM BADGE FRLG = BOULDER +
  EARNED BADGES FRLG = BOTH 3 — Celebi GBA frame with the Boulder Badge
  and three earned badges on the left and top.

**Performance**

- Cached path resolution. The mod no longer re-evaluates the full frame-
  selection tree on every frame. Previously each frame checked options,
  built asset paths, and probed the filesystem to confirm each candidate
  file existed — up to six file existence checks per frame during normal
  play. That work is now memoized. The selection is recomputed only when
  something that affects it actually changes: an option is edited, the
  player enters a new map, or the day/night period flips. The result is
  identical; only the wasted work is gone. Each layer has its own cache
  keyed on the options that affect it.
- Zero-cost idle rendering. When the base frame is NONE, no badge
  applies, and no icons are enabled, the render hook now returns before
  touching any graphics state. No canvas save, no scissor save, no color
  save, no restore. Nothing to draw means nothing is done.
- Correct SGB frame resolution on late game-version detection. The game
  version is now part of the cache key and is read from the live game
  object when the platform event hasn't delivered it, so if the SGB
  default frame is resolved before the game version becomes available,
  the correct frame is picked up automatically instead of being stuck on
  a fallback until the next option change.

These changes are most noticeable on lower-power devices with a frame,
badge, or icon active during normal gameplay.

**Supported games**

Red, Blue, Yellow, Gold, Silver, Crystal, FireRed, LeafGreen, Ruby,
Sapphire, Emerald.

**Display**

This version of the mod is optimized for the TrimUI Brick at 1024×768.
On that resolution every frame is pixel-perfect.

Other resolutions scale the artwork proportionally, and the result
depends on the specific device. If your screen is not 1024×768, the
frames will still display, but exact pixel alignment is not guaranteed.

All 4:3 screens have been updated to the new 4:3 viewport that ships
with gen1recomp v0.3.5 onwards.

This build represents the intended final quality level of the mod. Every
detail has been manually maximised within the author's capabilities.
That quality is specific to 1024×768; other resolutions are outside the
intended experience.

**16:9 and mobile devices**

Support for 16:9 and mobile screens has been removed in this version.
Automatic aspect ratio detection had a slight negative performance
impact on handhelds and offered little benefit, since their screens are
already 4:3. The process of reworking overlays for every aspect ratio
and screen position proved too complex to maintain alongside the 4:3
set.

If you are on a 16:9 or mobile device, use v1.0.4 instead. That release
contains partial 16:9 and mobile support, though it is incomplete and
was not fully tested on those screens.

Running a 4:3-only release on a non-4:3 screen will stretch the artwork.

**Testing**

All 4:3 functionality has been tested and is working on the TrimUI
Brick.

Feedback is welcome — through GitHub issues or the gen1recomp Discord
mod section. If you report from another device, please include your
device, resolution, and how the borders rendered.

**Notes**

- The mod platform does not support per-generation option schemas. A
  mod's options are defined once at load and cannot be filtered, hidden,
  or swapped based on the running game. That's why all sixteen option
  rows appear on every boot, including the rows that don't apply to the
  current generation. The row labels are the only signal.
- CONSOLE, PARTY GEN1-2, PKMN GEN1-2, PKMN GEN3, EARNED BADGES
  FRLG/RSE, GYM BADGE GEN1/2/FRLG/RSE, PKMN LOGO, POKEBALL,
  CENTER BALL GEN3, and RIGHT BALL GEN3 default to NONE/OFF, so the
  overlay is disabled on first launch to prevent the UI from being
  cropped on certain devices, which can make it difficult to navigate
  the settings menu. Set any row to a real value to enable the overlay.
- Changes apply live — no restart needed.
- Options save per save file. A fresh save starts at the mod's defaults.
  See "Saving per save file" above.
- The mod manager shows the last-used value for each option, not the
  current save's value. Per-save behavior is still honored when the
  frame is drawn — a save with POKEBALL = ON will show the ball even if
  the menu reads OFF — but the menu itself previews the last value you
  chose globally, not the value stored in the save you're currently
  playing. This is a limitation of the mod platform's option widget,
  which owns its own display state and does not read from the mod's
  per-save storage. If you want to confirm what a specific save is
  actually using, watch the frame itself: it always reflects that save's
  stored settings.
- Gen 1/2 and Gen 3 save separate settings. A frame chosen while playing
  Red never shows up on a FireRed boot, and vice versa.
- DAY/NIGHT applies to SGB, GB, and GBA frames. For SGB, it selects the
  day or night variant of the running game's frame and the themed
  Pokémon frames. For GB, it selects between the standard and dark Game
  Boy art. For GBA, it selects between the day and night art of the
  chosen console. All GBC frames are day-only, and PARTY overlays are
  day-only.
- Icons are console-aware. The POKEBALL row works on every console
  family that accepts icons (GB-family, GBA, GBA SP); CENTER BALL GEN3
  and RIGHT BALL GEN3 only draw when the console is GBA or GBA SP. The
  PKMN LOGO row resolves to the correct asset for the current console
  family. BALL SIZE GEN3 affects only the right-side GBA Pokéball. All
  icons are suppressed on SGB, SGB GOLD 97, and CONSOLE = NONE.
- Gym badges are supported on all eleven games. Badges draw on GB-family
  consoles for Gen 1 and Gen 2 games, and on GBA and GBA SP consoles for
  Gen 3 games. They are never drawn on SGB or SGB GOLD 97.
- Gen 2 gym badges are fully supported. On Gold, Silver, and Crystal,
  the GYM BADGE GEN2 row resolves to the correct Gold/Silver/Crystal
  badge art for all sixteen Johto and Kanto gyms. This includes Clair's
  gym at BLACKTHORN_GYM_1F and Blaine's relocated gym at SEAFOAM_GYM.
- Hoenn gym badges are fully supported. On Ruby, Sapphire, and Emerald,
  the GYM BADGE RSE row resolves to the correct Hoenn badge art for all
  eight gyms.
- Gold defaults to the standard Gold frame. To use the Spaceworld '97
  demo frame, select CONSOLE = SGB GOLD 97.
- PARTY GEN1-2 combines with CONSOLE. Set both to draw a party frame on
  a specific hardware variant. Setting PARTY GEN1-2 with CONSOLE = NONE,
  SGB, or SGB GOLD 97 shows a notice and draws the plain console frame.
- PARTY GEN1-2 wins over PKMN GEN1-2. If both are set, the party frame
  draws.
- PKMN GEN3 has no party equivalent. Party overlays are Gen 1/2 only.
- If CONSOLE = SGB and the running game can't be identified, no overlay
  is drawn. A notice appears on screen for 5 seconds asking you to pick
  a style manually.
- If a theme is set but CONSOLE is still NONE, no overlay is drawn and a
  notice appears for 5 seconds asking you to pick a console.
- If a frame file is missing, the mod draws the plain console frame and
  shows a notice explaining which file is missing. Nothing silently
  substitutes a different overlay.
- All border artwork is manually reworked by the author. No AI art was
  used.

**Installation**

1. Install the .zip through your mod manager, or copy the extracted
   folder into your mods directory.
2. Enable the mod in the launcher's MODS panel.
3. Launch any supported game. The overlay is off on first launch — the
   game screen will look normal.
4. Open the mod options, set CONSOLE (and optionally a theme, party,
   badge, or icon row), and the frame appears immediately.

**Updating**

This mod supports in-launcher updates. The launcher's MODS panel will
show an Update button when a newer release is available on GitHub. The
Versions button lets you pick any published release — useful if you need
to roll back to v1.0.4 for 16:9 or mobile use.

**Known bugs**

- AUTO (GYM) badge mode does not work on FireRed and LeafGreen yet. Use
  AUTO (CITY) or set the badge manually. AUTO (GYM) works on Gen 1 and
  Gen 2 games as before.
- AUTO (GYM) and AUTO (CITY) are untested on Hoenn games (Ruby,
  Sapphire, Emerald).

**Credits**

Borders and mod by BrazilKing, based on original SGB frames and GBC
Pokémon editions. PARTY overlays are community-requested, each based on
a contributor's current or favourite Gen 1/2 Pokémon.
