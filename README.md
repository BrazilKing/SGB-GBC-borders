**952,213,248,009 overlay combinations from 257 hand-drawn PNG files — no AI art.**

Two new earned-badge rows, a reworked Pokémon Center New York top logo,
cleaner menu labels, reordered choice lists, and simplified storage values.

Customizable GB, GBC, GBA, and SGB overlays for Gen 1, 2, and 3 in gen1recomp.

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

- Fully cached. No per-frame filesystem work.

- Console-aware. Every option resolves to the right art for the running game.

- 68% smaller install. 4.61 MB vs 14.6 MB in v1.3.7.

**FRAMES INCLUDED**

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

**BADGES**

- Forty gym badges. RBY Kanto (8), GSC Johto + Kanto (16), FRLG Kanto (8),
  RBSPEM Hoenn (8).

- Earned badges. RBY, GSC, FRLG, and RSE. Placements per game. AUTO modes
  that read the save.

- New in 1.5.0. EARNED LEFT/TOP and EARNED LR/BOTTOM G2 replace the
  single EARNED BADGE PLACEMENT row so Gen-1 and Gen-3 users don't see
  Gen-2-only options.

**ICONS**

- GEN1RECOMP logo, available on GB/GBC and GBA, left and top slots.

- NINTENDO logo, GB/GBC left and top slots.

- Pokémon logo, three variants: PKMN, PKMN B, PKMN C. GB/GBC left and top
  slots.

- Pokéball (console-aware).

- Left, center, and right Pokéballs. All three are separate toggles, each
  with its own screen position.

- Left and right ball sizes (LARGE, MEDIUM, SMALL, XL).

- BAR LOGO decoration. BOTH, LEFT, or TOP.

**OVERLAY COMBINATIONS**

The mod ships 257 PNG files and can produce 952,213,248,009 unique valid
overlays across all games.

The count is the product of every independent option that applies to a
given game, summed across all game classes.

- Gen 1 (Red, Blue, Yellow): 348,986,880,004 combinations

- Gen 2 (Gold, Silver, Crystal): 602,795,520,004 combinations

- Gen 3 Hoenn (Ruby, Sapphire, Emerald): 215,424,000 combinations

- FireRed / LeafGreen: 215,424,000 combinations

- Blank state (CONSOLE = OFF): 1

- Total: 952,213,248,009

This roughly doubles the 1.4.9 count of 476,106,624,009. The growth comes
entirely from splitting EARNED BADGE PLACEMENT (8 values) into two rows:

- EARNED LEFT/TOP (4 values)

- EARNED LR/BOTTOM G2 (4 values)

8 → 4 × 4 = 16. A ×2 jump on every game.

**PER-GAME CALCULATION**

Gen 1 and Gen 2 have the same structure.

The variables per non-SGB console are:

Frame content — 108

- 11 parties + 1 OFF, stacked with 8 themes + 1 OFF.

- Formula: 12 × 9 = 108.

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

- EARNED LEFT/TOP: 4.

- EARNED LR/BOTTOM G2: 4.

- EARNED COUNT: 17.

Gen 1 per-console breakdown

- GB: 108 × 2 × 216,000 × 11 × 16 × 17 = 139,594,752,000

- GB LIGHT: 69,797,376,000

- GB POCKET: 69,797,376,000

- GBC: 69,797,376,000

- SGB: 2 (day, night — base frame only)

- SGB GOLD 97: 2 (day, night — base frame only)

Gen 1 total: 348,986,880,004

Gen 2 per-console breakdown

- GB: 108 × 2 × 216,000 × 19 × 16 × 17 = 241,118,208,000

- GB LIGHT: 120,559,104,000

- GB POCKET: 120,559,104,000

- GBC: 120,559,104,000

- SGB: 2

- SGB GOLD 97: 2

Gen 2 total: 602,795,520,004

Gen 3 calculation

- Frame content: 5 (PKMN G3).

- Day / night: 2.

- Icons: 3,600 (BOTTOM LOGO (6) × LEFT LOGO (2) × TOP LOGO (6) ×
  LEFT BALL (5) × CENTER BALL (2) × RIGHT BALL (5)).

- Badge: 11.

- Earned LEFT/TOP: 4.

- Earned LR/BOTTOM G2: 4.

- Earned count: 17.

Per console:

- GBA: 5 × 2 × 3,600 × 11 × 16 × 17 = 107,712,000

- GBA SP: 107,712,000

Hoenn total: 215,424,000

FRLG total: 215,424,000

Grand total

- Blank state: 1

- 348,986,880,004 + 602,795,520,004 + 215,424,000 + 215,424,000 + 1
  = 952,213,248,009

The exact figure counts selectors like AUTO (GYM) and AUTO (CITY) as the
distinct choices they are.

Collapsing them to the badge images they resolve to yields a smaller
visual count.

**OPTIONS REFERENCE**

20 rows, always visible. Only the rows matching the running game are read.

Universal

CONSOLE — All games — default OFF

Selects the device frame.

Must be set to anything other than OFF for the overlay to draw.

- OFF

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

- Draws the Pokémon Center New York banner only when PKMN G3 is set to
  PKMNCENTER and no gym badge is active on the current map.

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

PARTY — Gen 1/2 — default OFF

Community-requested party frames.

Combines with CONSOLE to pick the hardware variant.

Stacks under PKMN G1-2: if both are set, the party frame draws first
and the themed character art draws on top.

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

PKMN G1-2 — Gen 1/2 — default OFF

Themed character art for GB / GBC consoles.

Stacks with PARTY.

- OFF

- CHIKORITA

- GEODUDE

- KANGASKHAN

- MEOWTH

- NIDOKING

- PIKACHU

- SPECIAL PIKACHU

- TOTODILE

Gen 3 frames

PKMN G3 — Gen 3 — default OFF

Themed character art for GBA / GBA SP consoles.

PKMNCENTER draws the Pokémon Center overlay on top of the console
background.

- OFF

- CELEBI

- LATIOS & LATIAS

- PKMNCENTER

- SUICUNE

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

EARNED LEFT/TOP — All — default OFF

Selects whether the LEFT and TOP earned badge layers draw.

LEFT draws the left column. TOP draws the top row. BOTH draws both.

- OFF

- LEFT

- TOP

- BOTH

EARNED LR/BOTTOM G2 — Gen 2 — default OFF

Selects whether the Gen-2-only LEFT&RIGHT and BOTTOM earned badge
layers draw.

LEFT&RIGHT draws the left and right columns. BOTTOM draws the bottom
row. BOTH draws both.

On Gen 1 and Gen 3 games, this row is ignored and only EARNED LEFT/TOP
draws.

- OFF

- LEFT&RIGHT

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

- Party — PARTY.

- Theme art — PKMN G1-2, drawn over the party.

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

- Theme art — PKMN G3.

- BOTTOM LOGO — device wordmark.

- TOP LOGO (NY banner when AUTO resolves or PKMN CT NY is selected).

- Gym badge.

- Earned badge.

SGB / SGB GOLD 97:

- Base frame only. Day or night variant.

No party, no theme art, no balls, no icons, no badges.

Rules:

- The three balls are the first layers after the body. Party and theme
  art draw over them.

- PARTY and PKMN G1-2 stack. The party frame draws first, then the
  themed character art on top.

- LED and BOTTOM LOGO draw over the party and theme art.

- BAR LOGO sits under LEFT LOGO and TOP LOGO.

- Left and top logos draw on top of the frame.

- Badges draw on top of everything.

- The PKMNCENTER theme draws as an overlay on the console background, so
  DAY/NIGHT applies.

- Explicit values that cannot be drawn on the current console or game
  generation show a short on-screen notice. AUTO and OFF never warn.

**AUTO BEHAVIOR**

- DAY/NIGHT. Picks day or night from the system clock (6am–6pm = day).
  Switches GB/GBC body, SGB border variant, and GBA background.

- BOTTOM LOGO. Follows the selected console on GB/GBC. Theme-aware on
  GBA: silver for most themes, gold for PKMNCENTER.

- LED. Follows the selected console: GB gets the plain LED, all others
  get the BATTERY LED.

- TOP LOGO AUTO. On GBA / GBA SP, draws the Pokémon Center New York
  banner only when PKMN G3 = PKMNCENTER and no gym badge is active on
  the current map. Otherwise silent. On GB / GBC, no-op.

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

- EARNED LR/BOTTOM G2. Gen 2 only. On Gen 1 and Gen 3, only EARNED
  LEFT/TOP draws.

- SGB. Base frame only. No party, theme, ball, icon, or badge layers.

- SGB GOLD 97. Flat frame, no themed overlays.

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

**MIGRATION FROM 1.4.9**

- NONE values remap to OFF on every row that previously used NONE.

- TOP LOGO NY values remap as follows:

    NY AUTO GEN3   → AUTO
    NY ALWAYS GEN3 → PKMN CT NY
    NY HIDDEN GEN3 → OFF

- All other rows carry their 1.4.9 values over unchanged.

- EARNED BADGE PLACEMENT does not carry over to EARNED LEFT/TOP or
  EARNED LR/BOTTOM G2. The player re-picks both rows once.

- Rolling back to 1.4.9 is not supported. The new keys are ignored by
  1.4.9, and the migration rewrites TOP LOGO on first read.

**TESTING**

All 4:3 functionality is tested on the TrimUI Brick.

Feedback welcome via GitHub issues or the gen1recomp Discord mod section.

If reporting from another device, please include your device, resolution,
and how the borders rendered.

**NOTES**

- The mod platform doesn't support per-generation schemas. All 20 rows
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
  SGB, SGB GOLD 97, and CONSOLE = OFF.

- Gym badges draw on GB-family consoles for Gen 1/2, and on GBA-family
  consoles for Gen 3. Never drawn on SGB.

- Options that do not apply to the current console or game generation
  show a short on-screen notice for 5 seconds when an explicit value is
  selected and cannot be drawn. AUTO and OFF never warn.

- The PKMNCENTER theme (previously POKEMON CENTER) draws on top of the
  console background instead of replacing it, so DAY/NIGHT applies to it
  correctly on both GBA and GBA SP.

- The PKMN Center New York top banner is a single asset shared between
  GBA and GBA SP. No SP-specific variant is required.

- All artwork is manually reworked by the author. No AI art was used.

**CREDITS**

Borders and mod by BrazilKing, based on original SGB frames and GBC
Pokémon editions.

PARTY overlays are community-requested, each based on a contributor's
current or favourite Gen 1/2 Pokémon.
