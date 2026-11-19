# Mailbox Almanac 1.0.0

**Thirteen letters a year, in the voice of the townsfolk, telling you what the calendar won't.**

The calendar costs more than a cow, and it only shows the season you're standing in. Meanwhile the things that actually cost you money — the festival you forgot, the crops that withered overnight, the fall you spent broke because you didn't save for seed — are things the game never puts in one place.

Mailbox Almanac fixes that the quiet way. A letter arrives at the turn of each season, and a shorter one a week in. Nothing else changes: no new items, no rebalancing, no menus, no HUD.

## Features

- **13 letters per year, repeating forever.** Opening letters cover the season's festivals and what to plant. Mid-season letters remind you about the things that need preparing. Closing letters are the practical ones — what dies at midnight, what to empty, what to repair while it's still cheap.
- **Written by the townsfolk, not a tutorial.** Lewis handles civic matters, Robin handles the season turning, Evelyn handles the dance and the feast, Willy handles summer, Pierre handles money, Marnie handles animals, Clint handles winter, Linus handles the last night of the year.
- **Every letter is a reminder you can act on.** Bring an ingredient to the Luau pot. Ask someone to the Flower Dance before the day of. Enter nine *different* things in the grange display instead of nine pumpkins. Clear the kegs before the season flips.
- **Works in existing saves.** Install mid-year and you'll get the next letter on schedule, and the full set from the following season.
- **English and Simplified Chinese included.** Language follows your game setting; translation is plain JSON in `i18n/`.
- **Pure Content Patcher.** No DLL, nothing to compile, nothing loaded into memory beyond two data assets.

## Installation

1. Install [SMAPI](https://smapi.io/) 4.0.0+ and [Content Patcher](https://www.nexusmods.com/stardewvalley/mods/1915) 2.0.0+.
2. Unzip `MailboxAlmanac-1.0.0.zip` into `Stardew Valley/Mods`. You should end up with `Mods/MailboxAlmanac/manifest.json`.
3. Play. The first letter arrives when the next day begins.

Requires Stardew Valley 1.6.15 or later.

## Notes

- The letters arrive on day 1, day 8 and day 28 of each season. If you skip the mailbox on those days, they'll still be sitting there.
- Deliveries are per-player and per-save; the letters are plain mail flags, so nothing extra is written into your save file.
- If you run another pack that rewrites `Data/TriggerActions` outright instead of patching it, the letters won't arrive — that's a conflict between the two packs, not something this one can work around.

## Changelog

### 1.0.0

- First release.
- 13 letters: welcome, plus opening / mid-season / closing for each of the four seasons.
- English and Simplified Chinese.
