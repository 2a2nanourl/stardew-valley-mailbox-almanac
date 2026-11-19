# Mailbox Almanac

A small content pack that puts a letter in your mailbox at the turn of every season, and a shorter one a week in. Thirteen letters, repeating every year, written in the voice of the townsfolk.

No new items, no rebalancing, no menus. Just the post.

## Why

The in-game calendar is expensive early on, and it only shows the season you're standing in. Most of the things players actually miss — the festival that snuck up, the last night to harvest before everything withers, the fact that fall is the season you should have saved seed money for — are things the game never tells you in one place.

So this pack tells you. It is deliberately quiet about it: one letter, in the mailbox you already check, at the moment it's useful.

## What's in the mailbox

| When | Letter | From |
| --- | --- | --- |
| First day after installing | About Your Mailbox | Lewis |
| Spring 1 / 8 / 28 | Spring Has Started · Five Days To The Egg Festival · Last Night Of Spring | Lewis · Evelyn · Robin |
| Summer 1 / 8 / 28 | Summer Is Here · Three Days To The Luau · Last Night Of Summer | Willy · Gus · Pierre |
| Fall 1 / 8 / 28 | Fall, And The Fair · Grange Display Reminder · Last Night Of Fall | Pierre · Lewis · Marnie |
| Winter 1 / 8 / 28 | Winter Work · Night Market And The Feast · Last Night Of Winter | Clint · Evelyn · Linus |

The opening letters cover the season's festivals and what to plant. The mid-season letters are reminders for whatever needs preparing — a dance partner, an ingredient for the soup pot, a grange display, a secret gift. The closing letters are the practical ones: what dies at midnight, what to empty, what to repair while it's cheap.

All thirteen repeat every year, including in saves that are already past year one.

## Requirements

- Stardew Valley **1.6.15** or later — current PC release is **1.6.16**, which this pack targets
- [SMAPI](https://smapi.io/) **4.0.0** or later
- [Content Patcher](https://www.nexusmods.com/stardewvalley/mods/1915) **2.0.0** or later

Written against 1.6.16 with Content Patcher 2.9.1. Everything it touches — `Data/Mail` and `Data/TriggerActions` — is stable across 1.6.x.

## Installation

1. Install SMAPI and Content Patcher.
2. Unzip `MailboxAlmanac-1.0.0.zip` into your `Stardew Valley/Mods` folder. You should end up with `Mods/MailboxAlmanac/manifest.json`.
3. Start the game. The first letter arrives the next time a day begins.

## Languages

English and Simplified Chinese are included; the game picks the one matching your language setting. Translation lives in `i18n/` — `default.json` and `zh.json`. Adding a language is a matter of copying `default.json`, translating the values, and naming the file after the language code.

## Compatibility

- Safe to add to an existing save. Nothing is stored in the save beyond the mail flags the letters themselves set.
- Compatible with mods that add their own mail or trigger actions; entries are namespaced under `2a2nanourl.MailboxAlmanac`.
- If you use a mod that rewrites `Data/TriggerActions` wholesale rather than patching it, the letters won't arrive. Patching mods are fine.
- Won't fire in multiplayer for farmhands other than the host's own mail — the letters are delivered to the player whose day starts.

## Uninstalling

Delete the `Mods/MailboxAlmanac` folder. Letters already in your mailbox stay readable; no new ones arrive.

## Credits

Letters written by 2a2nanourl. Thanks to Pathoschild for Content Patcher, and to the wiki editors whose documentation of `Data/Mail` and `Data/TriggerActions` made a pack like this possible without a line of C#.
