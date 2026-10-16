**77 trillion (77,111,823,744,972) overlay combinations from 284 hand-drawn PNG files — no AI art.**

Hand-reworked GB, GBC, GBA, and SGB overlays for every Gen 1, 2, and 3
game in gen1recomp. Twenty-two menu rows, fully stackable, per-save, live-
updating, and cached to the point where the mod costs two canvas blits
per frame no matter how much you enable. Off on first launch. Set
CONSOLE to anything other than OFF and the frame appears.

**CONTENTS**

- Quick start
- Features
- Frames included
- Badges
- Icons
- Overlay combinations
- Per-game calculation
- Options reference
- How options resolve
- AUTO behavior
- Per-save options
- Compatibility
- Display
- Known limitations
- Known bugs
- Performance
- Installation
- Updating
- Testing
- Notes
- Credits

**QUICK START**

- Install the .zip via your mod manager, or drop the extracted folder into
  your mods directory.

- Enable the mod in the launcher's MODS panel.

- Launch any supported game.

- Open the mod options, set CONSOLE, and the frame appears immediately.

The overlay is off on first launch. Set any row to a real value to enable it.

**FEATURES**

- 4:3 optimized, pixel-perfect on the TrimUI Brick (1024×768).

- Live updates. Changes apply from the mod manager with no restart.

- Per-save options. Each playthrough stores its own settings.

- Layered rendering. Body + balls + party + theme + LED + logo + bar +
  wordmarks + badge, all stackable.

- Fully cached. No per-frame filesystem work. Two canvas blits per frame.

- Console-aware. Every option resolves to the right art for the running game.

- 59% smaller install. 6 MB vs 14.6 MB in v1.3.7.

**FRAMES INCLUDED**

Gen 1/2

- SGB THEME row. Scrolls through 15 frames: AUTO (GAME), GOLD 97, RED,
  BLUE, YELLOW, GOLD, SILVER, CRYSTAL, CHIKORITA, GEODUDE, KANGASKHAN,
  MEOWTH, NIDOKING, PIKACHU, TOTODILE. Day and night variants for all.

  AUTO (GAME) resolves to the running game's own SGB border. GOLD 97 is
  the Spaceworld '97 demo border with the Pikablu night version. RED
  through CRYSTAL pin an official cart's border regardless of the running
  game. CHIKORITA through TOTODILE pin a themed overlay.

- GB / GBC device frames. GB, GB Light, GB Pocket, GBC, each with day and
  night body variants, plus themed variants.

- Eleven party overlays, split into left and right. PARTY L and PARTY R
  each scroll through the same eleven designs independently, so the two
  sides can differ. Community-requested frames.

- Twelve themed PKMN overlays, split into left and right. PKMN L and
  PKMN R each scroll through all twelve designs. The eight GB/GBC themes
  (Chikorita, Geodude, Kangaskhan, Meowth, Nidoking, Pikachu, Special
  Pikachu, Totodile) apply to Gen 1/2 games. The four GBA themes (Celebi,
  Suicune, PKMNCENTER, Latios & Latias) apply to Gen 3 games. The
  resolver routes to the correct asset folder for the running game and
  warns on a generation mismatch.

- Pokéball LED. Plain red, BATTERY variant, and a Pokéball-shaped "POWER"
  LED from the Special Pikachu edition.

Gen 3

- GBA / GBA SP device frames, day + night variants.

- Themed GBA frames. Celebi, Suicune, PKMNCENTER, Latios & Latias. Each
  split into left and right. All with day + night, GBA + GBA SP.

**BADGES**

- Forty gym badges. RBY Kanto (8), GSC Johto + Kanto (16), FRLG Kanto (8),
  RBSPEM Hoenn (8).

- Earned badges. RBY, GSC, FRLG, and RSE. Placements per game. AUTO modes
  that read the save.

- Two rows control earned badges:

  EARNED LEFT/LEFT&RIGHT groups the two columnar placements. LEFT draws
  the left column. LEFT&RIGHT draws the wide left-and-right band.

  EARNED TOP/BOTTOM groups the two horizontal placements. TOP draws the
  top row. BOTTOM draws the bottom row. BOTH draws both.

  LEFT&RIGHT and BOTTOM are Gen 2 only. On Gen 1 and Gen 3, selecting
  them shows a notice and no such badges are drawn.

**ICONS**

- GEN1RECOMP logo, available on GB/GBC and GBA, left and top slots.

- NINTENDO logo, GB/GBC left and top slots.

- Pokémon logo, three variants: PKMN, PKMN B, PKMN C. GB/GBC left and top
  slots.

- Pokémon Center NY banner, top-center on GBA / GBA SP. Shared asset
  between GBA and GBA SP.

- Pokéball (console-aware).

- Left, center, and right Pokéballs. All three are separate toggles, each
  with its own screen position.

- Left and right ball sizes (LARGE, MEDIUM, SMALL, XL).

- BAR LOGO decoration. BOTH, LEFT, or TOP.

**OVERLAY COMBINATIONS**

The mod ships 284 PNG files and can produce 77,111,823,744,972 unique
valid overlays across all games.

The count is the product of every independent option that applies to a
given game, summed across all game classes.

- Gen 1 (Red, Blue, Yellow): 28,267,937,280,030 combinations

- Gen 2 (Gold, Silver, Crystal): 48,826,437,120,030 combinations

- Gen 3 Hoenn (Ruby, Sapphire, Emerald): 807,840,000 combinations

- FireRed / LeafGreen: 807,840,000 combinations

- Blank state (CONSOLE = OFF): 1

- Total: 77,111,823,744,972

PARTY and PKMN each split into independent L and R rows, so the frame
content factor grew from 12 × 9 = 108 in v1.5.5 to
12 × 12 × 9 × 9 = 11,664 in v1.5.6 — a ×108 multiplier per Gen 1/2
console and ×5 per Gen 3 console (PKMN L × PKMN R alone).

The earned-badge placement block contributes 12 states
(EARNED LEFT/LEFT&RIGHT with 3 values × EARNED TOP/BOTTOM with 4 values)
instead of 16. LEFT&RIGHT is a single wide image that already covers both
columns, so LEFT + LEFT&RIGHT would double-draw the left column and is
not offered.

**PER-GAME CALCULATION**

Gen 1 and Gen 2 have the same structure.

The variables per non-SGB console are:

Frame content — 11,664

- PARTY L (11 + 1 OFF) × PARTY R (11 + 1 OFF) × PKMN L (8 + 1 OFF) ×
  PKMN R (8 + 1 OFF).

- Formula: 12 × 12 × 9 × 9 = 11,664.

Day / night

- 2 on GB.

- 1 elsewhere.

Icons — 216,000

- LED: 5.

- BOTTOM LOGO: 6 (GB/GBC values).

- LEFT LOGO: 6.

- TOP LOGO: 6.

- BAR LOGO: 4.

- LEFT BALL: 5.

- CENTER BALL: 2.

- RIGHT BALL: 5.

- Formula: 5 × 6 × 6 × 6 × 4 × 5 × 2 × 5 = 216,000.

Gym badge

- 11 for Gen 1.

- 19 for Gen 2.

Earned badge

- EARNED LEFT/LEFT&RIGHT: 3.

- EARNED TOP/BOTTOM: 4.

- Earned placement product: 3 × 4 = 12.

- EARNED COUNT: 17.

Gen 1 per-console breakdown

- GB: 11,664 × 2 × 216,000 × 11 × 12 × 17 = 11,307,174,912,000

- GB LIGHT: 5,653,587,456,000

- GB POCKET: 5,653,587,456,000

- GBC: 5,653,587,456,000

- SGB: 30 (SGB THEME × 15, day/night × 2 — base frame only)

Gen 1 total: 28,267,937,280,030

Gen 2 per-console breakdown

- GB: 11,664 × 2 × 216,000 × 19 × 12 × 17 = 19,530,574,848,000

- GB LIGHT: 9,765,287,424,000

- GB POCKET: 9,765,287,424,000

- GBC: 9,765,287,424,000

- SGB: 30

Gen 2 total: 48,826,437,120,030

Gen 3 calculation

- Frame content: 25 (PKMN G3 split into PKMN L × PKMN R, 5 × 5).

- Day / night: 2.

- Icons: 3,600 (BOTTOM LOGO (6) × LEFT LOGO (2) × TOP LOGO (6) ×
  LEFT BALL (5) × CENTER BALL (2) × RIGHT BALL (5)).

- Badge: 11.

- Earned LEFT/LEFT&RIGHT: 3.

- Earned TOP/BOTTOM: 4.

- Earned count: 17.

Per console:

- GBA: 25 × 2 × 3,600 × 11 × 12 × 17 = 403,920,000

- GBA SP: 403,920,000

Hoenn total: 807,840,000

FRLG total: 807,840,000

Grand total

- Blank state: 1

- 28,267,937,280,030 + 48,826,437,120,030 + 807,840,000 + 807,840,000 + 1
  = 77,111,823,744,972

The exact figure counts selectors like AUTO (GYM) and AUTO (CITY) as the
distinct choices they are.

Collapsing them to the badge images they resolve to yields a smaller
visual count.

**OPTIONS REFERENCE**

22 rows, always visible. Only the rows matching the running game are read.

Universal

CONSOLE — All games — default OFF

Selects the device frame.

Must be set to anything other than OFF for the overlay to draw.

- OFF

- GB

- SGB — SGB THEME row picks the frame

- GB POCKET

- GB LIGHT

- GBC

- GBA

- GBA SP

SGB THEME — Gen 1/2 on SGB — default AUTO (GAME)

Selects which SGB frame draws when CONSOLE = SGB.

AUTO (GAME) auto-resolves per game: Red, Blue, Yellow, Gold, Silver, or
Crystal each get their own SGB border. GOLD 97 forces the Spaceworld '97
demo border for every game. RED through CRYSTAL pin an official cart
regardless of the running game. CHIKORITA through TOTODILE pin a themed
overlay.

- AUTO (GAME)

- GOLD 97

- RED

- BLUE

- YELLOW

- GOLD

- SILVER

- CRYSTAL

- CHIKORITA

- GEODUDE

- KANGASKHAN

- MEOWTH

- NIDOKING

- PIKACHU

- TOTODILE

DAY/NIGHT — All games — default AUTO

AUTO picks from the system clock (6am–6pm = day).

On GB/GBC consoles it switches the body between grey and dark.

On SGB it selects the day or night variant of the SGB THEME frame.

On GBA it selects the light (day) or standard (night) background.

- AUTO

- DAY

- NIGHT

Frame-layer overrides

LED — GB / GBC family — default AUTO

Override or disable the power LED.

AUTO uses the plain LED on GB and the BATTERY LED on all others.

- AUTO

- GB

- GBC

- GBC SPECIAL PIKACHU

- OFF

BOTTOM LOGO — All — default AUTO

Override or disable the bottom-of-frame logo layer.

On GB/GBC, AUTO follows the selected console.

On GBA, AUTO is theme-aware: silver for most themes, gold for PKMNCENTER.

- AUTO

- OFF

- GB

- GB COLOR

- GB LIGHT

- GB POCKET

- PKMN CENTER

- PKMN CENTER SP

- GBA

- GBA SP

Logos

LEFT LOGO — All — default OFF

Logo drawn at the top-left position.

On GB/GBC: PKMN, PKMN B, PKMN C, NINTENDO, GEN1RECOMP.

On GBA: PKMN, GEN1RECOMP.

Stacks with TOP LOGO.

- OFF

- GEN1RECOMP

- NINTENDO

- PKMN

- PKMN B

- PKMN C

TOP LOGO — All — default AUTO

Logo drawn at the top-center position.

On GB/GBC: PKMN, PKMN B, PKMN C, NINTENDO, GEN1RECOMP.

On GBA: PKMN, GEN1RECOMP, plus AUTO and PKMN CT NY.

Stacks with LEFT LOGO.

- AUTO

- OFF

- GEN1RECOMP

- NINTENDO

- PKMN

- PKMN B

- PKMN C

- PKMN CT NY

AUTO behavior on GBA / GBA SP:

- Draws the Pokémon Center New York banner only when PKMN L or PKMN R is
  set to PKMNCENTER and no gym badge is active on the current map.

- In every other case AUTO draws nothing and stays silent.

PKMN CT NY forces the NY banner regardless of theme or active badge. The
banner asset is shared between GBA and GBA SP.

On GB / GBC consoles, AUTO is a no-op. PKMN CT NY shows a notice.

Bar

BAR LOGO — Gen 1/2 — default OFF

Bar decoration drawn on GB/GBC.

LEFT draws the left-edge bar, TOP draws the top-edge bar, BOTH draws both.

- OFF

- LEFT

- TOP

- BOTH

Balls

LEFT BALL — All — default OFF

Pokéball drawn at the top-left position.

On GB/GBC and GBA, the size is one of SMALL, MEDIUM, LARGE, XL.

Stacks with CENTER BALL and RIGHT BALL.

- OFF

- SMALL

- MEDIUM

- LARGE

- XL

CENTER BALL — All — default OFF

Pokéball drawn at the top-center position.

Console-aware: GB/GBC uses pokeball_gb_center, GBA uses
pokeball_gba_center.

Stacks with LEFT BALL and RIGHT BALL.

- OFF

- ON

RIGHT BALL — All — default OFF

Pokéball drawn at the top-right position.

On GB/GBC and GBA, the size is one of SMALL, MEDIUM, LARGE, XL.

- OFF

- SMALL

- MEDIUM

- LARGE

- XL

Gen 1/2 frames

PARTY L — Gen 1/2 — default OFF

Left-side community-requested party frame.

Stacks with PARTY R for the right side. If PARTY L and PARTY R are both
set, both draw. If only one is set, only that side draws.

Combines with CONSOLE to pick the hardware variant.

Stacks under PKMN L / PKMN R: if both are set, the party frame draws
first and the themed character art draws on top.

- OFF

- BLOODDLL

- BLOODDLL B

- DARTHTRON64

- FERNANDO

- FERNANDO B

- FOXEGORY5

- GRIMMNIR

- THEEON

- TORCHICISLAND

- TORCHICISLAND B

- ZEAK6464

PARTY R — Gen 1/2 — default OFF

Right-side community-requested party frame. Independent of PARTY L.

Same choices as PARTY L.

PKMN L — Gen 1/2 — default OFF

Left-side themed character art.

On Gen 1/2 games, the eight GB/GBC themes apply. On Gen 3 games, the four
GBA themes apply. Themes from the wrong generation produce a targeted
notice and nothing is drawn on that side.

Stacks with PKMN R for the right side.

- OFF

- CHIKORITA

- GEODUDE

- KANGASKHAN

- MEOWTH

- NIDOKING

- PIKACHU

- SPECIAL PIKACHU

- TOTODILE

- CELEBI

- LATIOS & LATIAS

- PKMNCENTER

- SUICUNE

PKMN R — Gen 1/2 — default OFF

Right-side themed character art. Independent of PKMN L.

Same choices as PKMN L.

Gym badges

GYM RBY — RBY — default AUTO (GYM)

AUTO (GYM) shows the badge inside its gym.

AUTO (CITY) shows it anywhere in the matching city.

Manual values force a specific badge.

- AUTO (CITY)

- AUTO (GYM)

- OFF

- BOULDER

- CASCADE

- THUNDER

- RAINBOW

- SOUL

- MARSH

- VOLCANO

- EARTH

GYM GSC — GSC — default AUTO (GYM)

Covers all sixteen Johto and Kanto gyms.

- AUTO (CITY)

- AUTO (GYM)

- OFF

- ZEPHYR

- HIVE

- PLAIN

- FOG

- STORM

- MINERAL

- GLACIER

- RISING

- BOULDER

- CASCADE

- THUNDER

- RAINBOW

- SOUL

- MARSH

- VOLCANO

- EARTH

GYM FRLG — FireRed / LeafGreen — default AUTO (GYM)

Kanto badges on GBA / GBA SP consoles.

- AUTO (CITY)

- AUTO (GYM)

- OFF

- BOULDER

- CASCADE

- THUNDER

- RAINBOW

- SOUL

- MARSH

- VOLCANO

- EARTH

GYM RSE — Ruby / Sapphire / Emerald — default AUTO (GYM)

Hoenn badges on GBA / GBA SP consoles.

- AUTO (CITY)

- AUTO (GYM)

- OFF

- STONE

- KNUCKLE

- DYNAMO

- HEAT

- BALANCE

- FEATHER

- MIND

- RAIN

Earned badges

EARNED LEFT/LEFT&RIGHT — All — default OFF

Selects which of the two columnar earned-badge placements draws.

LEFT draws the left column. LEFT&RIGHT draws the wide left-and-right
band. LEFT&RIGHT is Gen 2 only; on Gen 1 and Gen 3 it shows a notice
and nothing is drawn.

BOTH is not offered because LEFT&RIGHT already covers both columns;
drawing LEFT on top would double-render the left column.

- OFF

- LEFT

- LEFT&RIGHT

EARNED TOP/BOTTOM — All — default OFF

Selects which of the two horizontal earned-badge placements draws.

TOP draws the top row. BOTTOM draws the bottom row. BOTH draws both.
BOTTOM is Gen 2 only; on Gen 1 and Gen 3 it shows a notice and only
TOP draws.

- OFF

- TOP

- BOTTOM

- BOTH

EARNED COUNT — All — default AUTO

Selects how many badges to draw per active placement.

AUTO reads the save and draws exactly the earned badges.

A number caps at earned if the player has at least that many. If the
player has fewer, the mod draws all earned and pads the rest with the
lowest missing slots, with a warning.

- AUTO

- 1 through 16

**HOW OPTIONS RESOLVE**

Each overlay is a stack of layers, drawn in this order.

GB / GBC:

- Body — device background.

- Left ball.

- Center ball.

- Right ball.

- Party L — PARTY L.

- Party R — PARTY R.

- Theme art left — PKMN L, drawn over the party.

- Theme art right — PKMN R, drawn over the party.

- LED.

- BOTTOM LOGO — device wordmark.

- BAR LOGO.

- LEFT LOGO.

- TOP LOGO.

- Gym badge.

- Earned badge.

GBA / GBA SP:

- Body — device background.

- Left ball.

- Center ball.

- Right ball.

- Theme art left — PKMN L.

- Theme art right — PKMN R.

- BOTTOM LOGO — device wordmark.

- TOP LOGO (NY banner when AUTO resolves or PKMN CT NY is selected).

- Gym badge.

- Earned badge.

SGB:

- Base frame only — SGB THEME row picks which one. Day or night variant.

No party, no theme art, no balls, no icons, no badges.

Rules:

- The three balls are the first layers after the body. Party and theme
  art draw over them.

- PARTY L/R and PKMN L/R stack. The party frames draw first, then the
  themed character art on top.

- LED and BOTTOM LOGO draw over the party and theme art.

- BAR LOGO sits under LEFT LOGO and TOP LOGO.

- Left and top logos draw on top of the frame.

- Badges draw on top of everything.

- The PKMNCENTER theme draws as an overlay on the console background, so
  DAY/NIGHT applies.

- Explicit values that cannot be drawn on the current console or game
  generation show a short on-screen notice. AUTO and OFF never warn.

- SGB lists the frame-layer options it is ignoring in a single notice,
  and shows separate notices for logos and manual gym badges.

- All warnings on screen merge into a single wrapped, vertically growing
  box. Duplicate preamble sentences are removed. The box stays on
  screen long enough to read (4–10 seconds based on length).

**AUTO BEHAVIOR**

- CONSOLE = SGB. Auto-resolves per game via SGB THEME = AUTO (GAME):
  Red, Blue, Yellow, Gold, Silver, or Crystal each get their own SGB
  border. SGB THEME = GOLD 97 is a fixed override that always draws the
  Spaceworld '97 border. Any other SGB THEME value pins that specific
  frame regardless of the running game.

- DAY/NIGHT. Picks day or night from the system clock (6am–6pm = day).
  Switches GB/GBC body, SGB border variant, and GBA background.

- BOTTOM LOGO. Follows the selected console on GB/GBC. Theme-aware on
  GBA: silver for most themes, gold for PKMNCENTER.

- LED. Follows the selected console: GB gets the plain LED, all others
  get the BATTERY LED.

- TOP LOGO AUTO. On GBA / GBA SP, draws the Pokémon Center New York
  banner only when PKMN L or PKMN R is PKMNCENTER and no gym badge is
  active on the current map. Otherwise silent. On GB / GBC, no-op.

- AUTO (GYM). Reads the current map. Enters a gym = matching badge;
  leaves = no badge.

- AUTO (CITY). Same as AUTO (GYM) but extends to the whole city.

**PER-SAVE OPTIONS**

Options save per save file, not globally.

- A fresh save starts at the mod's defaults.

- Gen 1/2 and Gen 3 saves use separate buckets. A frame set on Red never
  appears on FireRed.

- Starting a new game gives you the defaults, not last session's
  selection.

Prior versions migrate automatically on first load:

- CONSOLE = SGB GOLD 97 migrates to CONSOLE = SGB + SGB THEME = GOLD 97.

- PARTY (v1.5.5) migrates into both PARTY L and PARTY R.

- PKMN G1-2 / PKMN G3 (v1.5.5) migrate into both PKMN L and PKMN R.

The mod manager menu shows the last-used value globally, not the current
save's value.

Per-save behavior is honored on-screen: if a save has LEFT BALL = LARGE,
the ball draws even if the menu reads OFF.

Watch the frame itself to confirm what a save is using.

**COMPATIBILITY**

Red / Blue / Yellow

- Gym badge: Kanto (RBY) ✅

- Earned badges: ✅

- Party frames: ✅

Gold / Silver / Crystal

- Gym badge: Johto + Kanto (GSC) ✅

- Earned badges: ✅

- Party frames: ✅

Ruby / Sapphire / Emerald

- Gym badge: Hoenn ✅

- Earned badges: Hoenn ✅

- Party frames: —

FireRed / LeafGreen

- Gym badge: Kanto (FRLG) ✅

- Earned badges: Kanto (FRLG) ✅

- Party frames: —

Console/theme mismatches (for example, GBA on a Gen 1 game) fall back to
the plain console frame and show a notice.

The same notice appears when an explicit option value cannot be drawn on
the current console or game generation.

AUTO and OFF never trigger a notice.

Nothing ever renders bare.

**DISPLAY**

Optimized for the TrimUI Brick at 1024×768. Other resolutions scale
proportionally, but pixel alignment isn't guaranteed.

All 4:3 screens use the 4:3 viewport from gen1recomp v0.3.5 onwards.

16:9 and mobile support has been removed.

Use v1.0.4 for partial 16:9/mobile support (incomplete, untested).

Running this 4:3 release on a non-4:3 screen will stretch the artwork.

**KNOWN LIMITATIONS**

- Party frames. Gen 1/2 only. Gen 3 games draw the base frame instead.
  SGB draws the base frame only.

- BAR LOGO. Gen 1/2 only.

- EARNED LEFT/LEFT&RIGHT and EARNED TOP/BOTTOM. LEFT&RIGHT and BOTTOM
  are Gen 2 only. On Gen 1 and Gen 3, selecting them shows a notice and
  no such badges are drawn.

- SGB. Base frame only. No party, theme, ball, icon, or badge layers.

- SGB THEME. Only applies when CONSOLE = SGB. On other consoles it is
  ignored and a notice is shown.

- NINTENDO, PKMN B, and PKMN C logos. GB/GBC only. There are no GBA
  variants.

- PKMN CT NY. GBA / GBA SP only. On GB / GBC the banner is not drawn
  and a notice is shown.

**KNOWN BUGS**

- AUTO (GYM). Does not work on FireRed / LeafGreen yet. Use AUTO (CITY)
  or set the badge manually.

- AUTO (GYM) and AUTO (CITY). Untested on Hoenn (Ruby, Sapphire,
  Emerald). Manual badge selection works.

**PERFORMANCE**

- Composite canvases. Frame layers, icons, and gym badge are baked into
  a single static canvas; earned badges are baked into a second canvas.
  Per-frame cost is two blits, regardless of how many layers are enabled.

- Static composite rebuilds only when its underlying paths change (option
  change, map change, day/night flip). Unrelated option changes cost
  nothing.

- Earned composite is built incrementally, a few PNGs per frame, and
  swapped in atomically when complete. Peak live textures for the earned
  layer is bounded regardless of badge count or how often the position
  options are changed.

- LRU canvas caches. Up to 4 recently-built canvases are kept per
  composite, so switching back to a previously-seen console, logo, gym,
  or earned-badge configuration is an instant lookup.

- Memoized keys. Composite keys are cached and only recomputed when the
  path list or backbuffer size changes. No per-frame string work.

- Throttled day/night sampling. The system clock is read twice per second
  instead of once per frame.

- LRU image cache. Every unique PNG the mod can draw is loaded once and
  reused. Ceiling of 96 entries comfortably covers every frame layer a
  single save can display at once, including the full PARTY / PKMN L/R
  theme set.

- Corrected release semantics. Only images the mod owns (loaded via raw
  LÖVE paths) are released on eviction; framework-cached images are
  dropped from the mod's table without release, since releasing them
  corrupts the framework's asset table.

- Asset loader chain. Tries love.graphics.newImage with common mount
  prefixes first, then FileData → ImageData → Image, then the framework
  loader as a last resort. A one-time log line reports which path was
  taken, so slow-fallback cases are visible in the log.

- Single read pass per rebuild. Every option a rebuild consults is read
  once via a single table, and asset existence checks are memoized for
  the session. Combined, a rebuild does roughly half the storage and
  filesystem lookups it used to.

- Zero-cost idle rendering. When nothing is drawn, the render hook
  returns before touching any graphics state.

- Warn-once per missing asset. A missing file logs exactly once, not once
  per frame.

- Event-driven cache invalidation. Cache rebuilds only on game.ready,
  mod.options_changed, map.entered, and day/night flip. That removes
  roughly 25 storage reads per frame from the previous design.

- Merged warning display. Frame, icon, gym, and earned-badge warnings
  collapse into one merged, word-wrapped, vertically growing box.
  Duplicate preamble sentences are removed. The box shows once per
  unique merged state and stays for 4–10 seconds depending on length.

Most noticeable on lower-power devices with a frame, badge, or icon
active.

**INSTALLATION**

- Install the .zip through your mod manager, or copy the extracted folder
  into your mods directory.

- Enable the mod in the launcher's MODS panel.

- Launch any supported game. The overlay is off on first launch.

- Open the mod options, set CONSOLE (and optionally a theme, party,
  badge, or icon row), and the frame appears.

**UPDATING**

The launcher's MODS panel shows an Update button when a newer release is
on GitHub.

The Versions button lets you roll back (for example, to v1.0.4 for
16:9/mobile).

**TESTING**

All 4:3 functionality is tested on the TrimUI Brick.

Feedback welcome via GitHub issues or the gen1recomp Discord mod section.

If reporting from another device, please include your device, resolution,
and how the borders rendered.

**NOTES**

- The mod platform doesn't support per-generation schemas. All 22 rows
  appear on every boot. The row labels are the only signal of which
  apply where.

- The overlay is off on first launch to prevent UI cropping on certain
  devices. Set any row to a real value to enable it.

- Changes apply live. No restart needed.

- Gen 1/2 and Gen 3 save separately.

- SGB auto-resolves per game via SGB THEME = AUTO (GAME). CONSOLE = SGB
  picks the correct border for Red, Blue, Yellow, Gold, Silver, or
  Crystal without any further setup. SGB THEME = GOLD 97 skips the auto
  selection and always draws the fixed GOLD 97 frame. Any other SGB
  THEME value pins that specific frame regardless of the running game.

- DAY/NIGHT applies to SGB, GB, GBC, and GBA frames. On GB/GBC consoles
  it switches the body between grey (day) and dark (night). On SGB it
  selects the day or night variant of the SGB THEME frame. On GBA it
  switches between the light and standard backgrounds.

- GBC supports day/night. GB, GB Light, GB Pocket, and GBC all use the
  same grey/dark body switching.

- The three balls are the first layers after the body. Party, theme art,
  LED, and logo all draw over them. Logos and badges draw on top of
  everything.

- SGB draws a single base frame. Party, theme art, balls, icons, and
  badges are suppressed on SGB.

- Icons are console-aware. LEFT BALL, CENTER BALL, and RIGHT BALL each
  render at their own screen position. LEFT BALL and RIGHT BALL carry
  their own size on both GB/GBC and GBA. All icons are suppressed on
  SGB and CONSOLE = OFF.

- Gym badges draw on GB-family consoles for Gen 1/2, and on GBA-family
  consoles for Gen 3. Never drawn on SGB.

- Options that do not apply to the current console or game generation
  show a short on-screen notice when an explicit value is selected and
  cannot be drawn. AUTO and OFF never warn.

- On SGB, frame-layer options that SGB cannot draw are listed in a single
  consolidated notice. Logo selections and manual gym badge selections
  each produce their own notice.

- All warnings on screen merge into one wrapped box. Frame, icon, gym,
  and earned channels combine into a single message; duplicate preamble
  sentences collapse. The box grows vertically to fit the text and stays
  on screen long enough to read.

- The PKMNCENTER theme (previously POKEMON CENTER) draws on top of the
  console background instead of replacing it, so DAY/NIGHT applies to it
  correctly on both GBA and GBA SP.

- The PKMN Center New York top banner is a single asset shared between
  GBA and GBA SP. No SP-specific variant is required.

- Reworked GBC Special Pikachu Edition overlay, brightness optimized.

- All artwork is manually reworked by the author. No AI art was used.

**CREDITS**

Borders and mod by BrazilKing, based on original SGB frames and GBC
Pokémon editions.

PARTY overlays are community-requested, each based on a contributor's
current or favourite Gen 1/2 Pokémon.
