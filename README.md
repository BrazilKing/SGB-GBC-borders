**8,243,269 overlay combinations from 154 hand-drawn PNG files — no AI art.**

Customizable GB, GBC, GBA, and SGB overlays for Gen 1, 2, and 3 in gen1recomp.

Quick start

    Install the .zip via your mod manager, or drop the extracted folder into your mods directory.

    Enable the mod in the launcher's MODS panel.

    Launch any supported game.

    Open the mod options, set CONSOLE, and the frame appears immediately.

The overlay is off on first launch — set any row to a real value to enable it.

Features

    4:3 optimized, pixel-perfect on the TrimUI Brick (1024×768)

    Live updates — changes apply from the mod manager with no restart

    Per-save options — each playthrough stores its own settings

    Layered rendering — body + LED + right ball + logo + party + theme + icons + gym badge + earned badges, all stackable

    Fully cached — no per-frame filesystem work

    Console-aware — every option resolves to the right art for the running game

    68% smaller install — 4.61 MB vs 14.6 MB in v1.3.7

Frames included

Gen 1/2

    Per-game automatic SGB borders (Red, Blue, Yellow, Gold, Silver, Crystal)

    Day and night variants, manual or auto

    GOLD 97 — Spaceworld '97 demo border with Pikablu night version

    Themed SGB overlays — Chikorita, Geodude, Kangaskhan, Meowth, Nidoking, Pikachu, Totodile (day + night), stacked on top of the base SGB border

    GB / GBC device frames — GB, GB Light, GB Pocket, GBC, each with day and night body variants, plus themed variants

    Nine party overlays — community-requested frames

    Nine themed frames — Chikorita, Geodude, Kangaskhan, Meowth, Nidoking, Pikachu, Special Pikachu, Totodile

    Pokéball LED — plain red, BATTERY variant, and a Pokéball-shaped "POWER" LED from the Special Pikachu edition

Gen 3

    GBA / GBA SP device frames — day + night variants

    Themed GBA frames — Celebi, Suicune, Pokémon Center, Latios & Latias — all with day + night, GBA + GBA SP

Badges

    Forty gym badges — RBY Kanto (8), GSC Johto + Kanto (16), FRLG Kanto (8), RBSPEM Hoenn (8)

    Earned badges — FRLG and RSE, left / top / both placements, AUTO modes that read the save

Icons

    Pokéball (console-aware)

    Pokémon logo

    Center and right Pokéballs — the right ball is now available on GB / GBC as well as GBA, with size control (Small / Medium / Large / XL)

Overlay combinations

The mod ships 154 PNG files and can produce 8,243,269 unique valid overlays across all games.

The count is the product of every independent option that applies to a given game, summed across all game classes.

    Gen 1 (Red, Blue, Yellow): 594,018 combinations

    Gen 2 (Gold, Silver, Crystal): 1,026,018 combinations

    Gen 3 Hoenn (Ruby, Sapphire, Emerald): 3,311,616 combinations

    FireRed / LeafGreen: 3,311,616 combinations

    Blank state (CONSOLE = NONE): 1

    Total: 8,243,269

Per-game calculation

Gen 1 and Gen 2 have the same structure. The variables per non-SGB console are:

    frame-content (18): 1 plain + 9 themes + 9 parties − 1 overlap (none counted twice)

    day/night (2 on GB, 1 elsewhere)

    icons (20): POKEBALL (2) × PKMN LOGO (2) × (right ball off × 1 + right ball on × 4 sizes)

    gym badge (11 for Gen 1, 19 for Gen 2)

    GB LOGO (6)

    LED (5)

Gen 1 per-console breakdown:

    GB: 18 × 2 × 20 × 11 × 6 × 5 = 237,600

    GB LIGHT: 18 × 1 × 20 × 11 × 6 × 5 = 118,800

    GB POCKET: 18 × 1 × 20 × 11 × 6 × 5 = 118,800

    GBC: 18 × 1 × 20 × 11 × 6 × 5 = 118,800

    SGB: 8 × 2 = 16 (base border + 7 themed overlays × day/night)

    SGB GOLD 97: 1 × 2 = 2 (base only, day/night)

Gen 1 total: 237,600 + 118,800 + 118,800 + 118,800 + 16 + 2 = 594,018

Gen 2 uses the same structure with 19 badge choices:

    GB: 18 × 2 × 20 × 19 × 6 × 5 = 410,400

    GB LIGHT: 18 × 1 × 20 × 19 × 6 × 5 = 205,200

    GB POCKET: 18 × 1 × 20 × 19 × 6 × 5 = 205,200

    GBC: 18 × 1 × 20 × 19 × 6 × 5 = 205,200

    SGB: 8 × 2 = 16

    SGB GOLD 97: 1 × 2 = 2

Gen 2 total: 410,400 + 205,200 + 205,200 + 205,200 + 16 + 2 = 1,026,018

Gen 3 uses a different formula. Frame-content is 7 (none + celebi + suicune + 3 Pokémon Center NY text states + latioslatias), icons are 64 (2 × 2 × 2 × 2 × 4), and GBA LOGO replaces GB LOGO/LED:

    GBA: 7 × 2 × 64 × 11 × 28 × 6 = 1,655,808

    GBA SP: 7 × 2 × 64 × 11 × 28 × 6 = 1,655,808

    Hoenn total: 3,311,616

    FRLG total: 3,311,616

Blank state: 1

Grand total: 594,018 + 1,026,018 + 3,311,616 + 3,311,616 + 1 = 8,243,269

The exact figure counts selectors like AUTO (GYM) and AUTO (CITY) as the distinct choices they are. Collapsing them to the badge images they resolve to yields a smaller visual count.

Options reference

20 rows, always visible. Only the rows matching the running game are read.

Universal

CONSOLE — All games — default NONE

Selects the device frame. Must be set to anything other than NONE for the overlay to draw.

    NONE

    GB

    SGB

    SGB GOLD 97

    GB POCKET

    GB LIGHT

    GBC

    GBA

    GBA SP

DAY/NIGHT — All games — default AUTO

AUTO picks from the system clock (6am–6pm = day). On GB/GBC consoles it switches the body between grey and dark. On SGB it selects the day or night variant of the per-game border. On GBA it selects the light (day) or standard (night) background.

    AUTO

    DAY

    NIGHT

Frame-layer overrides

GB LOGO — GB / GBC family — default AUTO

Override or disable the logo layer. AUTO follows the selected console.

    AUTO

    GAME BOY

    GAME BOY POCKET

    GAME BOY LIGHT

    GAME BOY COLOR

    OFF

LED — GB / GBC family — default AUTO

Override or disable the power LED. AUTO uses the plain LED on GB and the BATTERY LED on all others.

    AUTO

    GB

    GBC

    GBC SPECIAL PIKACHU

    OFF

GBA LOGO — GBA / GBA SP — default AUTO

Override or disable the GBA logo. AUTO is theme-aware — silver for most themes, gold for Pokémon Center.

    AUTO

    SILVER GBA

    SILVER GBA SP

    GOLD POKEMON CENTER

    GOLD POKEMON CENTER SP

    OFF

GBA NY TOP — GBA / GBA SP — default AUTO

Toggle the "Pokémon Center NEW YORK" top overlay. AUTO draws it only when the Pokémon Center theme is active and no badge is drawn. ALWAYS draws it on any GBA theme. HIDDEN suppresses it entirely.

    AUTO

    ALWAYS

    HIDDEN

Gen 1/2 frames

PARTY GEN1-2 — Gen 1/2 — default NONE

Community-requested party frames. Combines with CONSOLE to pick the hardware variant. Stacks under PKMN GEN1-2 — if both are set, the party frame draws first and the themed character art draws on top.

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

PKMN GEN1-2 — Gen 1/2 — default NONE

Themed character art for GB / GBC consoles. On SGB, the themed art is stacked on top of the base border.

    NONE

    CHIKORITA

    GEODUDE

    KANGASKHAN

    MEOWTH

    NIDOKING

    PIKACHU

    SPECIAL PIKACHU

    TOTODILE

Gen 3 frames

PKMN GEN3 — Gen 3 — default NONE

Themed character art for GBA / GBA SP consoles. Pokémon Center also draws the gold GBA logo and optional NY text.

    NONE

    CELEBI

    SUICUNE

    POKEMON CENTER

    LATIOS & LATIAS

Gen 3 badges

EARNED BADGES FRLG — FireRed / LeafGreen — default NONE

Left / top / both earned badge overlays. AUTO modes read the save and draw exactly the earned badges. Numbered modes force a count.

    NONE

    LEFT AUTO

    TOP AUTO

    BOTH AUTO

    LEFT 1 … LEFT 8

    TOP 1 … TOP 8

    BOTH 1 … BOTH 8

EARNED BADGES RSE — Ruby / Sapphire / Emerald — default NONE

Same structure as FRLG. AUTO modes are order-independent, so Emerald's out-of-order play draws correctly.

    NONE

    LEFT AUTO

    TOP AUTO

    BOTH AUTO

    LEFT 1 … LEFT 8

    TOP 1 … TOP 8

    BOTH 1 … BOTH 8

Gym badges

GYM BADGE GEN1 — RBY — default AUTO (GYM)

AUTO (GYM) shows the badge inside its gym. AUTO (CITY) shows it anywhere in the matching city. Manual values force a specific badge.

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

GYM BADGE GEN2 — GSC — default AUTO (GYM)

Covers all sixteen Johto and Kanto gyms, including Clair at BLACKTHORN_GYM_1F and Blaine at SEAFOAM_GYM.

    NONE

    AUTO (GYM)

    AUTO (CITY)

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

GYM BADGE FRLG — FireRed / LeafGreen — default AUTO (GYM)

Kanto badges on GBA / GBA SP consoles.

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

GYM BADGE RSE — Ruby / Sapphire / Emerald — default AUTO (GYM)

Hoenn badges on GBA / GBA SP consoles.

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

Icons

POKEBALL — All — default OFF

Draws the Pokéball icon. Console-aware — GB/GBC uses the standard ball, GBA uses the top-left ball.

    OFF

    ON

CENTER BALL — GBA only — default OFF

Draws the centered GBA Pokéball. There is no GB/GBC equivalent.

    OFF

    ON

RIGHT BALL — All consoles — default OFF

Draws the right-side Pokéball. Works on GB / GBC and GBA — the art is picked per console family.

    OFF

    ON

BALL SIZE — All consoles — default SMALL

Size of the right-side Pokéball. Ignored when RIGHT BALL is off.

    SMALL

    MEDIUM

    LARGE

    XL

PKMN LOGO — All — default OFF

Draws the Pokémon logo icon.

    OFF

    ON

How options resolve

Each overlay is a stack of layers, drawn in this order:

    Body — device background

    LED — GB / GBC power indicator

    Right ball — right-side Pokéball, on top of the LED, under the logo

    Logo — GB / GBC / GBA wordmark

    Party — Gen 1/2 only

    Theme art — character art on top of shared chrome

    Icons — Pokéball, Pokémon logo, GBA center ball

    Gym badge — Gen 1/2 GB-family, Gen 3 GBA

    Earned badges — Gen 3 GBA only

Rules:

    CONSOLE + PARTY combine — the console selects the hardware, the party row selects the contributor.

    PARTY and PKMN stack — the party frame draws first, then the themed character art on top. Both can be active at the same time.

    Icons and badges stack on top of the frame.

    GB LOGO / LED / GBA LOGO / GBA NY TOP override or disable the corresponding layer.

    SGB and SGB GOLD 97 have a flat base frame; SGB also supports themed overlays stacked on top.

AUTO behavior

DAY/NIGHT — Picks day or night from the system clock (6am–6pm = day). Switches GB/GBC body, SGB border variant, and GBA background.

GB LOGO — Follows the selected console — GB gets GAME BOY, GB POCKET gets GAME BOY POCKET, etc.

LED — Follows the selected console — GB gets the plain LED, all others get the BATTERY LED.

GBA LOGO — Theme-aware — silver for most themes, gold for Pokémon Center.

GBA NY TOP — Hides the NY overlay when a gym badge is active.

AUTO (GYM) — Reads the current map. Enters a gym = matching badge; leaves = no badge.

AUTO (CITY) — Same as AUTO (GYM) but extends to the whole city.

Per-save options

Options save per save file, not globally.

    A fresh save starts at the mod's defaults.

    Gen 1/2 and Gen 3 saves use separate buckets — a frame set on Red never appears on FireRed.

    Starting a new game gives you the defaults, not last session's selection.

Note: the mod manager menu shows the last-used value globally, not the current save's value. Per-save behavior is honored on-screen — if a save has POKEBALL = ON, the ball draws even if the menu reads OFF. Watch the frame itself to confirm what a save is using.

Compatibility

Red / Blue / Yellow

    Gym badge: Kanto (RBY) ✅

    Earned badges: —

    Party frames: ✅

Gold / Silver / Crystal

    Gym badge: Johto + Kanto (GSC) ✅

    Earned badges: —

    Party frames: ✅

Ruby / Sapphire / Emerald

    Gym badge: Hoenn ✅

    Earned badges: Hoenn ✅

    Party frames: —

FireRed / LeafGreen

    Gym badge: Kanto (FRLG) ✅

    Earned badges: Kanto (FRLG) ✅

    Party frames: —

Console/theme mismatches (e.g. GBA on a Gen 1 game) fall back to the plain console frame and show a notice — nothing ever renders bare.

Display

Optimized for the TrimUI Brick at 1024×768. Other resolutions scale proportionally, but pixel alignment isn't guaranteed.

All 4:3 screens use the 4:3 viewport from gen1recomp v0.3.5 onwards.

16:9 and mobile support has been removed. Use v1.0.4 for partial 16:9/mobile support (incomplete, untested). Running this 4:3 release on a non-4:3 screen will stretch the artwork.

Known limitations

    Party frames — Gen 1/2 only. Gen 3 games draw the base frame instead.

    Earned badges — FRLG and Hoenn only. Gen 1 and Gen 2 don't have an earned-badge layer yet.

    SGB GOLD 97 — flat frame, no themed overlays.

    CENTER BALL — GBA / GBA SP only. There is no GB/GBC center ball asset.

Known bugs

    AUTO (GYM) does not work on FireRed / LeafGreen yet. Use AUTO (CITY) or set the badge manually.

    AUTO (GYM) and AUTO (CITY) are untested on Hoenn (Ruby, Sapphire, Emerald). Manual badge selection works.

Performance

    Cached path resolution — no more filesystem probes per frame. Recomputed only on option change, map change, or day/night flip.

    LRU image cache — every unique PNG the mod can draw is loaded once and reused. No per-frame asset lookups during normal play.

    Zero-cost idle rendering — when nothing is drawn, the render hook returns before touching any graphics state.

    Correct SGB resolution even when the game version is detected late.

Most noticeable on lower-power devices with a frame, badge, or icon active.

Installation

    Install the .zip through your mod manager, or copy the extracted folder into your mods directory.

    Enable the mod in the launcher's MODS panel.

    Launch any supported game — the overlay is off on first launch.

    Open the mod options, set CONSOLE (and optionally a theme, party, badge, or icon row), and the frame appears.

Updating

The launcher's MODS panel shows an Update button when a newer release is on GitHub. The Versions button lets you roll back (e.g. to v1.0.4 for 16:9/mobile).

Testing

All 4:3 functionality is tested on the TrimUI Brick.

Feedback welcome via GitHub issues or the gen1recomp Discord mod section. If reporting from another device, please include your device, resolution, and how the borders rendered.

Notes

    The mod platform doesn't support per-generation schemas. All 20 rows appear on every boot — the row labels are the only signal of which apply where.

    The overlay is off on first launch to prevent UI cropping on certain devices. Set any row to a real value to enable it.

    Changes apply live — no restart needed.

    Gen 1/2 and Gen 3 save separately.

    DAY/NIGHT applies to SGB, GB, GBC, and GBA frames. On GB/GBC consoles it switches the body between grey (day) and dark (night); the logo and LED stay the same. On SGB it selects the day or night variant of the per-game border. On GBA it switches between the light and standard backgrounds. Party overlays are day-only.

    GBC supports day/night — GB, GB Light, GB Pocket, and GBC all use the same grey/dark body switching.

    Icons are console-aware. POKEBALL works on GB-family and GBA-family; CENTER BALL is GBA-only. RIGHT BALL works on both GB-family and GBA-family. BALL SIZE affects only the right-side ball. All icons are suppressed on SGB, SGB GOLD 97, and CONSOLE = NONE.

    Gym badges draw on GB-family consoles for Gen 1/2, and on GBA-family consoles for Gen 3. Never drawn on SGB.

    Modular console layers. GB LOGO, LED, and GBA LOGO let you override or disable individual chrome elements. GBA NY TOP toggles the Pokémon Center top overlay. Icons and badges stack on top of the frame.

    All artwork is manually reworked by the author. No AI art was used.

Credits

Borders and mod by BrazilKing, based on original SGB frames and GBC Pokémon editions. PARTY overlays are community-requested, each based on a contributor's current or favourite Gen 1/2 Pokémon.
