# Pet Owners

### UUID Definitions:&#x20;

**UUID** is the unique identification code that the game gives to a player or entity. Each player has their own that is the same across all of Minecraft. On its own, it often refers to the Hexadecimal UUID.

**Hexadecimal UUID** is the player's or entity's UUID, which is formatted in base 16 with hexadecimal numbers and leah.whaleterst. which may look like: `f81d4fae-7dec-11d0-a765-00a0c91e6bf6`\
**Int-array UUID** is the player's or entity's UUID, which is formatted as multiple numbers. It may look like `[I;812842158,521486673,-1593036876,-1491939852]`

**Floodgate UUID** is **t**he UUID that the server gives a bedrock player as a Hexadecimal UUID

## Getting Owner

While looking at an entity run `/data get entity {entity} Owner` . Replace {entity} with a target selector or the suggested UUID.

Copy the INT UUID and go to the [Minecraft UUID Converter](https://www.soltoder.com/mc-uuid-converter/) and paste that into the "UUID" section. A name should then appear. If the user is on bedrock you will need to copy the UUID and paste it into [MC Profile](https://mcprofile.io) as a floodgate UUID to find the player name.

{% hint style="info" %}
If you are on vanilla launcher, turn on the console in launcher settings. If on Prism or multiMC, open the instance Minecraft log. You can then coppy from there&#x20;
{% endhint %}

## Setting Owner

Find player's UUIDs or name. You can use apexs playerlist to search, `/plan search` , `/discord linked` or the Google Sheet, then use [MC Profile](https://mcprofile.io) to get the correct UUID (Floodgate UUID if on bedrock)

Use the [Minecraft UUID Converter](https://www.soltoder.com/mc-uuid-converter/) to convert the Hex UUID into an INT UUID

then run

`/data modify entity {entity} Owner set value {INT UUID}`

e.g. `/data modify entity 32feab4f-1ec3-4815-8f14-0a8d8aa0413f Owner set value [I;812842158,521486673,-1593036876,-1491939852]`

{% hint style="info" %}
You can find all the loaded pets owned by someone with this:

/effect give @e\[nbt={Owner: \[I; 0, 0, 590320, -2111244500]}] minecraft:glowing
{% endhint %}



{% embed url="https://mcprofile.io" %}
