# Creating Worlds

Visit the managing worlds and commands section of the wiki for more info

{% embed url="https://wiki.traincarts.net/index.php/MyWorlds" %}

You can create a world with the following command. You can find more detailed options [here](https://wiki.traincarts.net/p/MyWorlds/Commands#World_Creation).<br>

```
/world create worldname_environment(::options) (seed)
```

<details>

<summary>Examples</summary>

| Command                                                                 | Description                                                                       |
| ----------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| /world create world1                                                    | Creates a new overworld called 'world1'                                           |
| /world create world1\_nether                                            | Creates a new netherworld called 'world1\_nether'                                 |
| /world create mynether/nether                                           | Creates a new netherworld called 'mynether'                                       |
| /world create HippoCraft/flat 251                                       | Creates a new flatworld called 'HippoCraft' using seed 251                        |
| /world create waterworld/flat::2;7,5x1,5x3,5x12,90x9;1;biome\_1,village | Creates a flat waterworld                                                         |
| /world create Space:bSpace:awesome                                      | Create a spaceworld using the bSpace generator plugin with the 'awesome' settings |



</details>

{% hint style="warning" %}
Gamerules and difficulty are different in each world, so remember to set them
{% endhint %}

If you are doing a multiworld setup, make sure to merge the worlds like so. It is recommended that the first one is your main world, as inventories will be copied from the first world.&#x20;

```
/world inventory merge world world_nether world_the_end
/world lastposition merge world world_nether world_the_end
```

You can load the unload the world when you are done with the commands below

<pre><code><strong>/mw load worldname
</strong>/mw unload worldname
</code></pre>

```
/mw tp worldname
```
