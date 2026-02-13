---
icon: arrow-up-arrow-down
---

# Transferring accounts

This is useful if a player has gotten a new account or something like that. If players want to move to bedrock, that is a separate process that involves [linking them](https://link.geysermc.org). If doing the advanced techniques below, I recommend starting with those first.

~~If you want, you can use the~~ [~~google sheet~~](https://docs.google.com/spreadsheets/d/1RAVtTbTT8_WFFZVFMBG1g7GngSep1gQhg9ygU5Az1rU/edit) ~~for "security questions" before hand~~ (only with old whitelisting)

### Re-linking discord

run `/discord unlink <player/discord username/ID>` to unlink their account then they can join to re-link or you can force it with `/discord link` If they have the moderator role, they will automatically be given the luckperms group

### Transferring plots

You can tp to there plots the run `/plot setowner <player>` to change to the new one

### Inventory (Simple)

You can run `/irp restore <player>` then look in `Quits`, if that world is the smp, you can give them those items. Otherwise look in `Worlds` for they last went from an smp world to creative (it shows the data of the world it came from yet displays the name of the world they went to). You can take them out and give them to the player.

## Advanced

First you'll have to find the uuid (not trimmed) of the new and old player. I recommend using `/discord linked` or https://mcprofile.io to find them

### Player data & Inv

In the following folders, locate the old `<uuid>.dat` file and replace it with the uuid.

```lua
-- SMP
/default/paper_1_21_1_2972731/playerdata
/default/paper_1_21_1_2972731/advancements
/default/paper_1_21_1_2972731/stats
/default/paper_1_21_1_2972731_nether/DIM-1/playerdata

-- Plots251
/default/plots251/playerdata

-- Plots75
/default/plots75/playerdata
```

### Plugin data

_Some_ plugins follow a similar data pattern

```lua
-- Inventory RollBackPlus Backups
-- Rename folders
/default/plugins/InventoryRollbackPlus/backups/<type>

-- FAWE
/default/plugins/FastAsyncWorldEdit/clipboard
/default/plugins/FastAsyncWorldEdit/history

/default/plugins/VentureChat/PlayerData
/default/plugins/Essentials/userdata
```

I'm sure there may be more<br>

## Entites

Transferring pets and other data that is stored in blocks/entities must be done manually; check out [#setting-owner](../pet-owners.md#setting-owner "mention") for more details.
