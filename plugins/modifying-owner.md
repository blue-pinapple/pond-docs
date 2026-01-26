# Modifying Owner

If you are on vanilla launcher, turn on the console in launcher settings. If on Prism or multiMC, open the instance Minecraft log.&#x20;

find player's UUIDs or name. You can use apexs playerlist to search, `/plan search` , `/discord linked` or the Google Sheet&#x20;

Use [https://mcprofile.io](https://mcprofile.io) to find the bedrock UUID and look for the floodgate UUID



/data get entity {entity} Owner

Then use the converter to find the owner and confirm it is correct

{% embed url="https://www.soltoder.com/mc-uuid-converter/" %}

Then use that to convert the new player to the I format

run this command to set.

/data modify entity {entity} Owner set value {UUID in I format}

e.g.&#x20;

```
/data modify entity 32feab4f-1ec3-4815-8f14-0a8d8aa0413f Owner set value [I;812842158,521486673,-1593036876,-1491939852]
```

{% hint style="info" %}
You can find all the pets owned by someone with this:

/effect give @e\[nbt={Owner: \[I; 0, 0, 590320, -2111244500]}] minecraft:glowing
{% endhint %}



{% embed url="https://mcprofile.io" %}
