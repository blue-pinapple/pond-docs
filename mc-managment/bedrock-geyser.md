---
icon: cube
---

# Bedrock/Geyser

**Geyser** allows Bedrock clients to join Java servers. It's known as a packet translator. **Floodgate** is a proxy that allows the bedrock accounts to join without a Java one. All players who join through floodgate have a `.` prefix at the start of their gamertag. e.g. the player `gamer3523` will be seen as `.gamer3523` to the game.

## Getting User info

You can use [MC Profile](https://mcprofile.io/) to get more info about a Bedrock user and their Geyser information.

## Bedrock and Java

If someone wants to add their Bedrock account, discuss whether they want to link, add, or [transferring-accounts.md](transferring-accounts.md "mention").

### Linking

Bedrock players can link to their Java account. This means that when they join, they will join using their Java account, effectively "syncing" the two. If their bedrock account was their main, make sure to transfer as much data over as possible [transferring-accounts.md](transferring-accounts.md "mention"). The bedrock data will be inaccessible until they unlink again.



Get players to go to [link.geysermc.org](https://link.geysermc.org) and choose how they wish to link. If their bedrock and java are on the same Microsoft account, I recommend the online account linking method.

{% hint style="info" %}
Global whitelisting enabled. If they have linked before, it will already be "syncing"
{% endhint %}

### Whitelisting/Alt

DiscordSRV should handle most of the whitelisting, but if a player wants an alt bedrock or it isn't working, you may need to manually whitelist them. You can do this with the command `/fwhitelist add`   &#x20;
