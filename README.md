798,717 overlay combinations from 222 hand-drawn PNG files — no AI art.

Customizable GB, GBC, GBA, SGB, and Hoenn overlays for Gen 1, 2, and 3 in gen1recomp.
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

    Layered rendering — frame + icons + gym badge + earned badges, all stackable

    Fully cached — no per-frame filesystem work

    Console-aware — every option resolves to the right art for the running game

Frames included
Gen 1/2

    Per-game automatic SGB borders (Red, Blue, Yellow, Gold, Silver, Crystal)

    Day and night variants, manual or auto

    GOLD 97 — Spaceworld '97 demo border with Pikablu night version

    Themed SGB frames — Chikorita, Geodude, Kangaskhan, Meowth, Nidoking, Pikachu, Totodile (day + night)

    GB / GBC device frames — GB, GB Light, GB Pocket, GBC, plus themed variants

    Nine party overlays — community-requested frames in GB, GB Dark, GB Light, GB Pocket, GBC variants

Gen 3

    GBA / GBA SP device frames — day + night variants

    Themed GBA frames — Celebi, Suicune, Pokémon Center, Latios & Latias — all with day + night, GBA + GBA SP

Badges

    Forty gym badges — RBY Kanto (8), GSC Johto + Kanto (16), FRLG Kanto (8), RBSPEM Hoenn (8)

    Earned badges — FRLG and RSE, left / top / both placements, AUTO modes that read the save

Icons

    Pokéball (console-aware)

    Pokémon logo

    GBA-only center / right Pokéballs with size control (Small / Medium / Large / XL)

Overlay combinations

The mod ships 222 PNG files and can produce 798,717 unique valid overlays across all games.
Game	Valid combinations
Gen 1 (Red, Blue, Yellow)	3,758
Gen 2 (Gold, Silver, Crystal)	6,478
Gen 3 Hoenn (Ruby, Sapphire, Emerald)	394,240
FireRed / LeafGreen	394,240
Blank state (CONSOLE = NONE)	1
Total	798,717

After collapsing selectors that resolve to the same image (AUTO (GYM), AUTO (CITY), LEFT/TOP/BOTH AUTO, BALL SIZE GEN3), the mod produces approximately 368,877 distinct composited screens.
Options reference

16 rows, always visible. Only the rows matching the running game are read.
Universal
Row	Choices
CONSOLE	NONE, GB, SGB, SGB GOLD 97, GB POCKET, GB LIGHT, GBC, GBA, GBA SP
DAY/NIGHT	AUTO, DAY, NIGHT
Gen 1/2
Row	Choices
PARTY GEN1-2	NONE + 9 community overlays
PKMN GEN1-2	NONE + Chikorita, Geodude, Kangaskhan, Meowth, Nidoking, Pikachu, Totodile
Gen 3
Row	Choices
PKMN GEN3	NONE + Celebi, Suicune, Pokémon Center, Latios & Latias
EARNED BADGES FRLG	NONE, LEFT/TOP/BOTH AUTO, LEFT/TOP/BOTH 1–8
EARNED BADGES RSE	NONE, LEFT/TOP/BOTH AUTO, LEFT/TOP/BOTH 1–8
Gym badges
Row	Choices
GYM BADGE GEN1	NONE, AUTO (GYM), AUTO (CITY), 8 Kanto badges
GYM BADGE GEN2	NONE, AUTO (GYM), AUTO (CITY), 8 Johto + 8 Kanto GSC badges
GYM BADGE FRLG	NONE, AUTO (GYM), AUTO (CITY), 8 Kanto badges
GYM BADGE RSE	NONE, AUTO (GYM), AUTO (CITY), 8 Hoenn badges
Icons
Row	Choices
PKMN LOGO	OFF, ON
POKEBALL	OFF, ON
CENTER BALL GEN3	OFF, ON (GBA only)
RIGHT BALL GEN3	OFF, ON (GBA only)
BALL SIZE GEN3	SMALL, MEDIUM, LARGE, XL

Defaults are NONE / OFF, except the four gym badge rows which default to AUTO (GYM).
How options resolve

Each overlay is a stack of up to four layers:
text

4. Earned badges    (Gen 3 GBA only)
3. Gym badge        (Gen 1/2 GB-family, Gen 3 GBA)
2. Icons            (Pokéball, logo, center/right balls)
1. Frame            (device, theme, or party)

    CONSOLE + PARTY combine — the console selects the hardware, the party row selects the contributor.

    PARTY overrides PKMN — if both are set, the party frame wins.

    Icons and badges stack on top of the frame.

Auto badge behavior

AUTO (GYM) reads the current map. Entering a gym draws the matching badge; leaving removes it.

    Gen 1 and FRLG follow the Kanto gym order.

    Gen 2 follows Johto first, then Kanto — includes Clair at BLACKTHORN_GYM_1F and Blaine at his relocated SEAFOAM_GYM.

    Hoenn follows the eight Hoenn gyms.

AUTO (CITY) extends this to the whole city. Entering Pewter City shows the Boulder Badge and keeps it visible anywhere in Pewter.

Manual mode forces a specific badge regardless of map.
Per-save options

Options save per save file, not globally.

    A fresh save starts at the mod's defaults.

    Gen 1/2 and Gen 3 saves use separate buckets — a frame set on Red never appears on FireRed.

    Starting a new game gives you the defaults, not last session's selection.

Note: the mod manager menu shows the last-used value globally, not the current save's value. Per-save behavior is honored on-screen — if a save has POKEBALL = ON, the ball draws even if the menu reads OFF. Watch the frame itself to confirm what a save is using.
Compatibility
Game	Gym badge	Earned badges	Party frames
Red / Blue / Yellow	✅ Kanto (RBY)	—	✅
Gold / Silver / Crystal	✅ Johto + Kanto (GSC)	—	✅
Ruby / Sapphire / Emerald	✅ Hoenn	✅ Hoenn	—
FireRed / LeafGreen	✅ Kanto (FRLG)	✅ Kanto (FRLG)	—

Console/theme mismatches (e.g. GBA on a Gen 1 game) fall back to the plain console frame and show a notice — nothing ever renders bare.
Display

Optimized for the TrimUI Brick at 1024×768. Other resolutions scale proportionally, but pixel alignment isn't guaranteed.

All 4:3 screens use the 4:3 viewport from gen1recomp v0.3.5 onwards.

16:9 and mobile support has been removed. Use v1.0.4 for partial 16:9/mobile support (incomplete, untested). Running this 4:3 release on a non-4:3 screen will stretch the artwork.
Known limitations

    Party frames are Gen 1/2 only. Gen 3 games draw the base frame instead.

    Earned badges are FRLG and Hoenn only. Gen 1 and Gen 2 don't have an earned-badge layer yet.

    Console/theme mismatches fall back to the plain frame with a notice.

Known bugs

    AUTO (GYM) does not work on FireRed / LeafGreen yet. Use AUTO (CITY) or set the badge manually.

    AUTO (GYM) and AUTO (CITY) are untested on Hoenn (Ruby, Sapphire, Emerald). Manual badge selection works.

Performance

    Cached path resolution — no more filesystem probes per frame. Recomputed only on option change, map change, or day/night flip.

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

    The mod platform doesn't support per-generation schemas. All 16 rows appear on every boot — the row labels are the only signal of which apply where.

    The overlay is off on first launch to prevent UI cropping on certain devices. Set any row to a real value to enable it.

    Changes apply live — no restart needed.

    Gen 1/2 and Gen 3 save separately.

    DAY/NIGHT applies to SGB, GB, and GBA frames. All GBC frames are day-only; party overlays are day-only.

    Icons are console-aware. POKEBALL works on GB-family and GBA-family; CENTER BALL GEN3 and RIGHT BALL GEN3 are GBA-only. BALL SIZE GEN3 affects only the right-side ball. All icons are suppressed on SGB, SGB GOLD 97, and CONSOLE = NONE.

    Gym badges draw on GB-family consoles for Gen 1/2, and on GBA-family consoles for Gen 3. Never drawn on SGB.

    All artwork is manually reworked by the author. No AI art was used.

Credits

Borders and mod by BrazilKing, based on original SGB frames and GBC Pokémon editions. PARTY overlays are community-requested, each based on a contributor's current or favourite Gen 1/2 Pokémon.
