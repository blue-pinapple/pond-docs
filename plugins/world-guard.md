---
description: How to make member's build areas and other World Guard info
---

# World Guard

World Guard is a system that allows regions to have unique build/interaction permissions. The Core part of WorldGuard is Regions. I highly recommend reading the wiki (especially the highlighted sections) if you want to change flags.

{% embed url="https://worldguard.enginehub.org/en/latest/regions/" %}

{% hint style="warning" %}
World Guad does not have tab autocomplete. Use their wiki to help guide you.
{% endhint %}



## Member's-only build area

### Creating

Select an area with the world edit wand tool (wooden axe). Create a region, then set it to inherit from `member_only_template`. Note: the name is **not** plural. If a world doesn't have `member_only_template`  region, you may need to create one.

{% code title="Replace <region> with the name you wish that area to have" %}
```lua
/region define <region>
/region setparent <region> member_only_template
```
{% endcode %}

If you wish to change the flags for this region only, run a command like the one below. Note: this will not change the flags of any other member region. To do that, continue reading.

```lua
/rg flag <region> <flag> <allow/deny>
```

### Template Settings

Modifying the flags of the template is easy. All children **in that world** will inherit these permissions unless it has been set for themselves.

```lua
/rg flag members_only_template <flag> <allow/deny>
```

#### Current Settings (as of writing)

{% hint style="info" %}
global regions (member\_only\_template) are world-specific, so these may differ slightly. Run `/region info member_only_template` for updated info
{% endhint %}

Anyone in the `paid-member` group is automatically added as a member to this group.

```
/rg addmember member_only_template g:paid-member
```

flags (all others are defaults):

{% code title="Global (not member spesfic)" %}
```
greeting: Now entering member's build zone
```
{% endcode %}

nonplayer-protection-domains



## Command cheat sheet

{% code overflow="wrap" %}
```lua
/region flags <region> list --Interactive list of flags
/region list --Lists all regions of that world 
/rg addmember member_only_template g:paid-member
/region define -g member_only_template --Create member only region (look at current settings and set)
```
{% endcode %}
