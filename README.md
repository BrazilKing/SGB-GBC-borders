476,106,624,009 overlay combinations from 257 hand-drawn PNG files — no AI art.

Full earned badge coverage across all three generations, three new Pokémon
logo variants, a resizable left Pokéball, a performance overhaul, and a
cleaner menu.

Customizable GB, GBC, GBA, and SGB overlays for Gen 1, 2, and 3 in gen1recomp.

CONTENTS

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

QUICK START

- Install the .zip via your mod manager, or drop the extracted folder into
  your mods directory.

- Enable the mod in the launcher's MODS panel.

- Launch any supported game.

- Open the mod options, set CONSOLE, and the frame appears immediately.

The overlay is off on first launch. Set any row to a real value to enable it.

FEATURES

- 4:3 optimized, pixel-perfect on the TrimUI Brick (1024×768).

- Live updates. Changes apply from the mod manager with no restart.

- Per-save options. Each playthrough stores its own settings.

- Layered rendering. Body + balls + party + theme + LED + logo + bar +
  wordmarks + badge, all stackable.

- Fully cached. No per-frame filesystem work.

- Console-aware. Every option resolves to the right art for the running game.

- 68% smaller install. 4.61 MB vs 14.6 MB in v1.3.7.

FRAMES INCLUDED

Gen 1/2

- Per-game automatic SGB borders (Red, Blue, Yellow, Gold, Silver, Crystal).

- Day and night variants, manual or auto.

- GOLD 97. Spaceworld '97 demo border with Pikablu night version.

- GB / GBC device frames. GB, GB Light, GB Pocket, GBC, each with day and
  night body variants, plus themed variants.

- Eleven party overlays. Community-requested frames.

- Eight themed frames. Chikorita, Geodude, Kangaskhan, Meowth, Nidoking,
  Pikachu, Special Pikachu, Totodile.

- Pokéball LED. Plain red, BATTERY variant, and a Pokéball-shaped "POWER"
  LED from the Special Pikachu edition.

Gen 3

- GBA / GBA SP device frames, day + night variants.

- Themed GBA frames. Celebi, Suicune, PKMNCENTER, Latios & Latias. All
  with day + night, GBA + GBA SP.

BADGES

- Forty gym badges. RBY Kanto (8), GSC Johto + Kanto (16), FRLG Kanto (8),
  RBSPEM Hoenn (8).

- Earned badges. RBY, GSC, FRLG, and RSE. Placements per game. AUTO modes
  that read the save.

ICONS

- GEN1RECOMP logo, available on GB/GBC and GBA, left and top slots.

- NINTENDO logo, GB/GBC left and top slots.

- Pokémon logo, three variants: PKMN, PKMN B, PKMN C. GB/GBC left and top
  slots.

- Pokéball (console-aware).

- Left, center, and right Pokéballs. All three are separate toggles, each
  with its own screen position.

- Left and right ball sizes (LARGE, MEDIUM, SMALL, XL).

- BAR GEN1-2 decoration. BOTH, LEFT, or TOP.

OVERLAY COMBINATIONS

The mod ships 257 PNG files and can produce 476,106,624,009 unique valid
overlays across all games.

The count is the product of every independent option that applies to a
given game, summed across all game classes.

- Gen 1 (Red, Blue, Yellow): 174,493,440,004 combinations

- Gen 2 (Gold, Silver, Crystal): 301,397,760,004 combinations

- Gen 3 Hoenn (Ruby, Sapphire, Emerald): 107,712,000 combinations

- FireRed / LeafGreen: 107,712,000 combinations

- Blank state (CONSOLE = NONE): 1

- Total: 476,106,624,009

PER-GAME CALCULATION

Gen 1 and Gen 2 have the same structure.

The variables per non-SGB console are:

Frame content — 108

- 11 parties + 1 NONE, stacked with 8 themes + 1 NONE.

- Formula: 12 × 9 = 108.

Day / night

- 2 on GB.

- 1 elsewhere.

Icons — 216,000

- LED GEN1-2: 5.

- BOTTOM LOGO: 6 (GB/GBC values).

- LEFT LOGO: 6.

- TOP LOGO: 6.

- BAR GEN1-2: 4.

- LEFT BALL: 5.

- CENTER BALL: 2.

- RIGHT BALL: 5.

- Formula: 5 × 6 × 6 × 6 × 4 × 5 × 2 × 5 = 216,000.

Gym badge

- 11 for Gen 1.

- 19 for Gen 2.

Earned badge

- EARNED BADGE PLACEMENT: 8.

- EARNED BADGE COUNT: 17.

Gen 1 per-console breakdown

- GB: 108 × 2 × 216,000 × 11 × 8 × 17 = 69,797,376,000

- GB LIGHT: 34,898,688,000

- GB POCKET: 34,898,688,000

- GBC: 34,898,688,000

- SGB: 2 (day, night — base frame only)

- SGB GOLD 97: 2 (day, night — base frame only)

Gen 1 total: 174,493,440,004

Gen 2 per-console breakdown

- GB: 108 × 2 × 216,000 × 19 × 8 × 17 = 120,559,104,000

- GB LIGHT: 60,279,552,000

- GB POCKET: 60,279,552,000

- GBC: 60,279,552,000

- SGB: 2

- SGB GOLD 97: 2

Gen 2 total: 301,397,760,004

Gen 3 calculation

- Frame content: 5 (PKMN GEN3).

- Day / night: 2.

- Icons: 3,600 (BOTTOM LOGO (6) × LEFT LOGO (2) × TOP LOGO (6) ×
  LEFT BALL (5) × CENTER BALL (2) × RIGHT BALL (5)).

- Badge: 11.

- Earned placement: 8.

- Earned count: 17.

Per console:

- GBA: 5 × 2 × 3,600 × 11 × 8 × 17 = 53,856,000

- GBA SP: 53,856,000

Hoenn total: 107,712,000

FRLG total: 107,712,000

Grand total

- Blank state: 1

- 174,493,440,004 + 301,397,760,004 + 107,712,000 + 107,712,000 + 1
  = 476,106,624,009

The exact figure counts selectors like AUTO (GYM) and AUTO (CITY) as the
distinct choices they are.

Collapsing them to the badge images they resolve to yields a smaller
visual count.

Gen 3 NY text states also collapse, because 4 non-PKMNCENTER themes treat
AUTO and HIDDEN identically.

OPTIONS REFERENCE

19 rows, always visible. Only the rows matching the running game are read.

Universal

CONSOLE — All games — default NONE

Selects the device frame.

Must be set to anything other than NONE for the overlay to draw.

- NONE

- GB

- SGB

- SGB GOLD 97

- GB POCKET

- GB LIGHT

- GBC

- GBA

- GBA SP

DAY/NIGHT — All games — default AUTO

AUTO picks from the system clock (6am–6pm = day).

On GB/GBC consoles it switches the body between grey and dark.

On SGB it selects the day or night variant of the per-game border.

On GBA it selects the light (day) or standard (night) background.

- AUTO

- DAY

- NIGHT

Frame-layer overrides

LED GEN1-2 — GB / GBC family — default AUTO

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

- GAME BOY

- GAME BOY COLOR

- GAME BOY LIGHT

- GAME BOY POCKET

- GOLD POKEMON CENTER

- GOLD POKEMON CENTER SP

- OFF

- SILVER GBA

- SILVER GBA SP

Logos

LEFT LOGO — All — default OFF

Logo drawn at the top-left position.

On GB/GBC: PKMN, PKMN B, PKMN C, NINTENDO, GEN1RECOMP.

On GBA: PKMN, GEN1RECOMP.

Stacks with TOP LOGO.

- GEN1RECOMP

- NINTENDO

- OFF

- PKMN

- PKMN B

- PKMN C

TOP LOGO — All — default OFF

Logo drawn at the top-center position.

On GB/GBC: PKMN, PKMN B, PKMN C, NINTENDO, GEN1RECOMP.

On GBA: PKMN, GEN1RECOMP, plus NY AUTO GEN3, NY ALWAYS GEN3,
NY HIDDEN GEN3.

Stacks with LEFT LOGO.

- GEN1RECOMP

- NINTENDO

- NY AUTO GEN3

- NY ALWAYS GEN3

- NY HIDDEN GEN3

- OFF

- PKMN

- PKMN B

- PKMN C

Bar

BAR GEN1-2 — Gen 1/2 — default OFF

Bar decoration drawn on GB/GBC.

LEFT draws the left-edge bar, TOP draws the top-edge bar, BOTH draws both.

- BOTH

- LEFT

- OFF

- TOP

Balls

LEFT BALL — All — default OFF

Pokéball drawn at the top-left position.

On GB/GBC and GBA, the size is one of LARGE, MEDIUM, SMALL, XL.

Stacks with CENTER BALL and RIGHT BALL.

- LARGE

- MEDIUM

- OFF

- SMALL

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

On GB/GBC and GBA, the size is one of LARGE, MEDIUM, SMALL, XL.

- LARGE

- MEDIUM

- OFF

- SMALL

- XL

Gen 1/2 frames

PARTY GEN1-2 — Gen 1/2 — default NONE

Community-requested party frames.

Combines with CONSOLE to pick the hardware variant.

Stacks under PKMN GEN1-2: if both are set, the party frame draws first
and the themed character art draws on top.

- BLOODDLL

- BLOODDLL B

- DARTHTRON64

- FERNANDO

- FERNANDO B

- FOXEGORY5

- GRIMMNIR

- NONE

- THEEON

- TORCHICISLAND

- TORCHICISLAND B

- ZEAK6464

PKMN GEN1-2 — Gen 1/2 — default NONE

Themed character art for GB / GBC consoles.

Stacks with PARTY GEN1-2.

- CHIKORITA

- GEODUDE

- KANGASKHAN

- MEOWTH

- NIDOKING

- NONE

- PIKACHU

- SPECIAL PIKACHU

- TOTODILE

Gen 3 frames

PKMN GEN3 — Gen 3 — default NONE

Themed character art for GBA / GBA SP consoles.

PKMNCENTER draws the Pokémon Center overlay on top of the console
background.

- CELEBI

- LATIOS & LATIAS

- NONE

- PKMNCENTER

- SUICUNE

Gym badges

GYM BADGE RBY — RBY — default AUTO (GYM)

AUTO (GYM) shows the badge inside its gym.

AUTO (CITY) shows it anywhere in the matching city.

Manual values force a specific badge.

- AUTO (CITY)

- AUTO (GYM)

- BOULDER

- CASCADE

- EARTH

- MARSH

- NONE

- RAINBOW

- SOUL

- THUNDER

- VOLCANO

GYM BADGE GSC — GSC — default AUTO (GYM)

Covers all sixteen Johto and Kanto gyms.

- AUTO (CITY)

- AUTO (GYM)

- BOULDER (GSC)

- CASCADE (GSC)

- EARTH (GSC)

- FOG

- GLACIER

- HIVE

- MARSH (GSC)

- MINERAL

- NONE

- PLAIN

- RAINBOW (GSC)

- RISING

- SOUL (GSC)

- STORM

- THUNDER (GSC)

- VOLCANO (GSC)

- ZEPHYR

GYM BADGE FRLG — FireRed / LeafGreen — default AUTO (GYM)

Kanto badges on GBA / GBA SP consoles.

- AUTO (CITY)

- AUTO (GYM)

- BOULDER

- CASCADE

- EARTH

- MARSH

- NONE

- RAINBOW

- SOUL

- THUNDER

- VOLCANO

GYM BADGE RSE — Ruby / Sapphire / Emerald — default AUTO (GYM)

Hoenn badges on GBA / GBA SP consoles.

- AUTO (CITY)

- AUTO (GYM)

- BALANCE

- DYNAMO

- FEATHER

- HEAT

- KNUCKLE

- MIND

- NONE

- RAIN

- STONE

Earned badges

EARNED BADGE PLACEMENT — All — default OFF

Selects which placements draw earned badges.

LEFT/TOP works on all generations.

LEFT&RIGHT GEN2 and BOTTOM GEN2 are Gen 2 only.

- ALL

- BOTTOM GEN2

- LEFT&RIGHT GEN2

- LEFT&RIGHT GEN2 + BOTTOM GEN2

- LEFT/TOP

- LEFT/TOP + BOTTOM GEN2

- LEFT/TOP + LEFT&RIGHT GEN2

- OFF

EARNED BADGE COUNT — All — default AUTO

Selects how many badges to draw per active placement.

AUTO reads the save and draws exactly the earned badges.

A number caps at earned if the player has at least that many. If the
player has fewer, the mod draws all earned and pads the rest with the
lowest missing slots, with a warning.

- AUTO

- 1 through 16

HOW OPTIONS RESOLVE

Each overlay is a stack of layers, drawn in this order.

GB / GBC:

- Body — device background.

- Left ball.

- Center ball.

- Right ball.

- Party — PARTY GEN1-2.

- Theme art — PKMN GEN1-2, drawn over the party.

- LED GEN1-2.

- BOTTOM LOGO — device wordmark.

- BAR GEN1-2.

- LEFT LOGO.

- TOP LOGO.

- Gym badge.

- Earned badge.

GBA / GBA SP:

- Body — device background.

- Left ball.

- Center ball.

- Right ball.

- Theme art — PKMN GEN3.

- BOTTOM LOGO — device wordmark.

- TOP LOGO (NY banner when an NY value is selected).

- Gym badge.

- Earned badge.

SGB / SGB GOLD 97:

- Base frame only. Day or night variant.

No party, no theme art, no balls, no icons, no badges.

Rules:

- The three balls are the first layers after the body. Party and theme
  art draw over them.

- PARTY and PKMN GEN1-2 stack. The party frame draws first, then the
  themed character art on top.

- LED and BOTTOM LOGO draw over the party and theme art.

- BAR GEN1-2 sits under LEFT LOGO and TOP LOGO.

- Left and top logos draw on top of the frame.

- Badges draw on top of everything.

- The PKMNCENTER theme draws as an overlay on the console background, so
  DAY/NIGHT applies.

- Explicit values that cannot be drawn on the current console or game
  generation show a short on-screen notice.

AUTO BEHAVIOR

- DAY/NIGHT. Picks day or night from the system clock (6am–6pm = day).
  Switches GB/GBC body, SGB border variant, and GBA background.

- BOTTOM LOGO. Follows the selected console on GB/GBC. Theme-aware on
  GBA: silver for most themes, gold for PKMNCENTER.

- LED GEN1-2. Follows the selected console: GB gets the plain LED, all
  others get the BATTERY LED.

- NY AUTO GEN3. Draws the NY banner only when the PKMNCENTER theme is
  active and no badge is drawn.

- AUTO (GYM). Reads the current map. Enters a gym = matching badge;
  leaves = no badge.

- AUTO (CITY). Same as AUTO (GYM) but extends to the whole city.

PER-SAVE OPTIONS

Options save per save file, not globally.

- A fresh save starts at the mod's defaults.

- Gen 1/2 and Gen 3 saves use separate buckets. A frame set on Red never
  appears on FireRed.

- Starting a new game gives you the defaults, not last session's
  selection.

The mod manager menu shows the last-used value globally, not the current
save's value.

Per-save behavior is honored on-screen: if a save has LEFT BALL = LARGE,
the ball draws even if the menu reads OFF.

Watch the frame itself to confirm what a save is using.

COMPATIBILITY

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

AUTO, OFF, and NONE never trigger a notice.

Nothing ever renders bare.

DISPLAY

Optimized for the TrimUI Brick at 1024×768. Other resolutions scale
proportionally, but pixel alignment isn't guaranteed.

All 4:3 screens use the 4:3 viewport from gen1recomp v0.3.5 onwards.

16:9 and mobile support has been removed.

Use v1.0.4 for partial 16:9/mobile support (incomplete, untested).

Running this 4:3 release on a non-4:3 screen will stretch the artwork.

KNOWN LIMITATIONS

- Party frames. Gen 1/2 only. Gen 3 games draw the base frame instead.
  SGB draws the base frame only.

- BAR GEN1-2. Gen 1/2 only.

- LEFT&RIGHT GEN2 and BOTTOM GEN2 earned badge placements. Gen 2 only.

- SGB. Base frame only. No party, theme, ball, icon, or badge layers.

- SGB GOLD 97. Flat frame, no themed overlays.

- NINTENDO, PKMN B, and PKMN C logos. GB/GBC only. There are no GBA
  variants.

KNOWN BUGS

- AUTO (GYM). Does not work on FireRed / LeafGreen yet. Use AUTO (CITY)
  or set the badge manually.

- AUTO (GYM) and AUTO (CITY). Untested on Hoenn (Ruby, Sapphire,
  Emerald). Manual badge selection works.

PERFORMANCE

- Cached path resolution. No more filesystem probes per frame. Recomputed
  only on option change, map change, or day/night flip.

- LRU image cache. Every unique PNG the mod can draw is loaded once and
  reused. No per-frame asset lookups during normal play.

- Zero-cost idle rendering. When nothing is drawn, the render hook
  returns before touching any graphics state.

- Correct SGB resolution even when the game version is detected late.

- Warn-once per missing asset. A missing file logs exactly once, not once
  per frame.

- Event-driven cache invalidation. Cache rebuilds only on game.ready,
  mod.options_changed, map.entered, and day/night flip. That removes
  roughly 25 storage reads per frame from the previous design.

- Image cache capped at 64 entries. Every frame the mod can draw fits in
  the cache, so nothing evicts during normal play.

- Frame, badge, icon, and earned-badge resolvers each have their own
  warning slot. Up to four notices stack on screen, each shown once per
  unique message for 5 seconds.

Most noticeable on lower-power devices with a frame, badge, or icon
active.

INSTALLATION

- Install the .zip through your mod manager, or copy the extracted folder
  into your mods directory.

- Enable the mod in the launcher's MODS panel.

- Launch any supported game. The overlay is off on first launch.

- Open the mod options, set CONSOLE (and optionally a theme, party,
  badge, or icon row), and the frame appears.

UPDATING

The launcher's MODS panel shows an Update button when a newer release is
on GitHub.

The Versions button lets you roll back (for example, to v1.0.4 for
16:9/mobile).

TESTING

All 4:3 functionality is tested on the TrimUI Brick.

Feedback welcome via GitHub issues or the gen1recomp Discord mod section.

If reporting from another device, please include your device, resolution,
and how the borders rendered.

NOTES

- The mod platform doesn't support per-generation schemas. All 19 rows
  appear on every boot. The row labels are the only signal of which
  apply where.

- The overlay is off on first launch to prevent UI cropping on certain
  devices. Set any row to a real value to enable it.

- Changes apply live. No restart needed.

- Gen 1/2 and Gen 3 save separately.

- DAY/NIGHT applies to SGB, GB, GBC, and GBA frames. On GB/GBC consoles
  it switches the body between grey (day) and dark (night). On SGB it
  selects the day or night variant of the per-game border. On GBA it
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
  SGB, SGB GOLD 97, and CONSOLE = NONE.

- Gym badges draw on GB-family consoles for Gen 1/2, and on GBA-family
  consoles for Gen 3. Never drawn on SGB.

- Options that do not apply to the current console or game generation
  show a short on-screen notice for 5 seconds when an explicit value is
  selected and cannot be drawn. AUTO, OFF, and NONE never warn.

- The PKMNCENTER theme (previously POKEMON CENTER) draws on top of the
  console background instead of replacing it, so DAY/NIGHT applies to it
  correctly on both GBA and GBA SP.

- All artwork is manually reworked by the author. No AI art was used.

CREDITS

Borders and mod by BrazilKing, based on original SGB frames and GBC
Pokémon editions.

PARTY overlays are community-requested, each based on a contributor's
current or favourite Gen 1/2 Pokémon.
