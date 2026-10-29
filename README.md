# KCD2 Companion

The full suite for **Kingdom Come: Deliverance II**, in one window inside the game (**F6**) or a browser panel on a second screen.

**Skip has had real problems, and we're fixing them one by one.** In earlier versions, many Skips didn't do what playing does: a skipped conversation could sit on a black screen, a skipped fight could end with enemies still standing, a skipped hand-over could leave the item in the chest. In 1.4.9 the panel marked 520 Skips **risky**: ones we already knew didn't match play.

**What we're doing about it.** We're replaying every quest in the real game, step by step, and checking each Skip against what happens when you play it yourself. When a Skip does something different, we fix it so it uses the game's own conversation, fight or hand-over, or we take that Skip out. 1.5.0 is the biggest update so far, with more than 110 of those fixes.

**Where it stands at 1.5.0.** KCD2's 205 quests have 2,382 Skips, one for every way a step can end. We've checked 767 of them and finished 25 quests from start to end. The risky list is down from 520 to 385. Testing also finds problems in Skips that weren't marked risky, so keep a save from before any Skip you care about, or use **Go** and play that part.

**What's next.** Version 2.0, once every quest has been checked.

- **Quests**: go straight to your current objective, or skip the busywork up to the next real decision. An objective that can end more than one way shows each ending; the choice stays yours.
- **Items**: all 5,120, laid out like a shop, best first with their damage, armour and price. Give yourself any of them, or go to where one is sold or lying.
- **Me**: Henry's health, stamina, stats, skills and money.
- **Cheat modes**: God mode, infinite stamina, never hungry or tired, unseen and unheard, run faster, hit harder, gear never wears, carry more, learn faster.
- **Achievements**: all 83, with the quest that grants each. Unlock any of them.
- **People, places and chests**: go to any of them, or bring a person to you.
- **Misc**: save anywhere without Saviour Schnapps, bring your horse, and **F8** jumps to the quest you're tracking.

![The F6 window: Quests](screenshots/quests.png)

| | |
|---|---|
| ![Me](screenshots/me.png) | ![Cheat modes](screenshots/misc.png) |
| ![Items](screenshots/items.png) | ![Achievements](screenshots/achievements.png) |

## Features

- **Quests**: every current objective with **Go** (to its marker), **Summon** (when the marker is a person) and **Skip**. Skip fires what completes the objective in play, read from the game's own quest data: a conversation's outcome happens as if you had had it (the item it hands over, where people go, the next objective), a cutscene or a conversation the game starts itself plays, choices left to you, and a world event happens as if it had. Where it is known to leave something undone, the button reads **Skip (risky)**, its tooltip says what is missed, and it asks before skipping. **Skip to next decision** completes the safe ones one step at a time and stops at a risky one, a decision, a conversation or a scene, then takes you there. Views of every objective and every open ending.
- **Items**: all 5,120 in a category bar like the inventory's (weapons, armour and clothing, horse, food and drink, potions, herbs and crafting, books and maps, tools, dice, other), each category in the groups you look for: swords to firearms, helmet to boots, healing to poison, skill books by skill and volume. Best first, with the damage, defence, power, noise, charisma or nourishment and the price beside each name, as the inventory shows them at the item's best quality. **Give** any quantity, of one item or (**Give all**) of every colour and pattern it comes in; **Go** to the shops, chests and spots one can be had, nearest first.
- **Achievements**: all 83 Steam achievements with your earned state, each with the quest that grants it where the game says; **Unlock** sets an unearned one on your Steam account.
- **Me**: health, stamina, nourishment and energy (refill one or all), groschen in steps up to +10,000, the four attributes and fifteen skills (+1 / +5 / Max).
- **Misc**: Save now (no schnapps), Bring my horse, and nine **cheat modes**: God mode, Infinite stamina, Never hungry or tired, Unseen and unheard, Run twice as fast, Hit twice as hard, Gear never wears, Carry far more, Learn three times as fast.
- **People**: everyone loaded around you, by in-game name, with Go and Summon.
- **Places**: villages, towns, monasteries and camps with their shops, smithies, alchemy tables, grindstones, baths, barbers and beds; **Mark** and **Back**; type an X and a Y to go to any point of the map, with where you stand shown beside them.
- **Chests**: every container in the level, locked ones marked.
- **Views** on every long list: items that can be had somewhere, quest items, what is in your bag, A to Z; locked, unlocked or stocked chests; people within 50 m; shops or services only.
- **F8** goes to the tracked quest's nearest current objective.
- Jumps work on foot and on horseback, land on the floor under roofs and trees, and never inside a trigger area.
- **Languages**: follows your game's language setting. The Companion's own words are in English, Chinese, French and German; a game set to any other language gets English. Names of people, places, items, quests and journal lines always come from the game's own text, in whatever language it runs.

## Quest skips: read this

A skip completes an objective without playing it, and it has to leave the world the way playing it would. KCD2's quests are long chains of conversations, scenes, fights and objects, and later steps read what each one left behind: who is alive and where they are, what was said, what Henry carries, whether a crime was seen. The game has no modding interface for any of this, so every pattern has to be found and tested by hand, and every quest is being tested step by step on several machines. The panel marks about 385 of the game's 2,382 objective endings **Skip (risky)**, where we know a skip cannot yet do what play does, and asks before those; the testing keeps finding problems in other skips too. About 120 have no Skip: the game sets them in a way the trainer cannot trigger, or they are cut content that never comes up. A skip that goes wrong can leave leftovers in your save, such as a later quest that never gets its marker, and the only way back is a save from before it. Keep a save from before any skip you care about, or use **Go** and play that part.

## Install

**Installer**: download **`KCD2-Companion-1.5.0-Installer.exe`** from the [latest release](../../releases) and run it. It finds the game on Steam, GOG or Epic (or paste the game folder), installs with one click, updates and uninstalls, and shows the panel in its own window while the game runs. Windows may warn about an unknown publisher: More info > Run anyway.

**Manual**: download **`KCD2-Companion-1.5.0.zip`** from the same release and extract it into the game folder (Steam: right-click the game > Manage > Browse local files), keeping its folders. Start the game and load a save; press **F6**, or open **http://127.0.0.1:17602** in a browser on the same PC. `INSTALL.txt` in the zip lists every file it adds; deleting them uninstalls it. A `Mods\mod_order.txt` (mod managers write one) makes the game load only the mods it lists; the plugin adds the Companion to it.

**GOG and Epic** (untested): the installer puts the files beside that store's `KingdomCome.exe`. By hand: the game runs from `Bin\Win64MasterMasterGogPGO\` (Epic: `Bin\Win64MasterMasterEpicPGO\`). Extract the zip into the game folder as above, then move what it put in `Bin\Win64MasterMasterSteamPGO\` into that folder, next to `KingdomCome.exe`.

**Game Pass** (untested): `INSTALL.txt` says where each piece goes. The installer handles Steam, GOG and Epic.

Also on Nexus Mods: https://www.nexusmods.com/kingdomcomedeliverance2/mods/3812 and the [Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=3821323940) (the window and panel still need the plugin from the installer or the zip).

## Compatibility

Built and tested on Steam build **1.5.6** (23914554). The plugin reads the game's quest objects at fixed offsets, so a game update may need a rebuilt plugin. GOG's build 15693 is the same game version as Steam 1.5.6. The GOG, Epic and Game Pass builds are handled from published information and not yet tested; there the Achievements tab says it needs Steam. Test on a copy of your save first.

## Also by me

- **Sandrock Companion** for My Time at Sandrock: the full suite: quests, items, achievements, stats and money, cheat modes, people, places and chests. [GitHub](https://github.com/registered2nd/sandrock-companion) · [Nexus Mods](https://www.nexusmods.com/mytimeatsandrock/mods/173)
- **KCD Companion** for Kingdom Come: Deliverance: the full suite: quests, items, achievements, Henry's stats and money, cheat modes, people, places and chests; Quest Autopilot is part of it. [GitHub](https://github.com/registered2nd/kcd-companion) · [Nexus Mods](https://www.nexusmods.com/kingdomcomedeliverance/mods/2406)

## Credits

Original mod code. The cheat modes' buff technique (a mod's own `buff__<mod>.xml` and the engine's stat codes) follows [kcd2-cheat](https://github.com/pryans/kcd2-cheat). Uses Ultimate ASI Loader (MIT) to load the plugin, Dear ImGui (MIT), MinHook (BSD-2), nlohmann/json (MIT) and kcd2db's CryEngine headers (MIT). Not affiliated with Warhorse Studios or Deep Silver.
