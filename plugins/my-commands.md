---
description: Plugin that manages custom commands. (replacement of CustomCommands)
---

# My Commands

Offical Documentation: [https://dev.bukkit.org/projects/mycommand/pages/configuration-and-example](https://dev.bukkit.org/projects/mycommand/pages/configuration-and-example)

## Folder Structure

The main folder can be found at `/default/plugins/MyCommand`

The main folder consists of multiple configs relating to storing data/varibales (these are mostly unused. (Honestly, all the configs are default).

The commands folder is where you will do most of the changes. Each YAML document is a collection of commands i.e. one file can have multiple commands.

<div><figure><img src="../.gitbook/assets/Screenshot 2025-12-31 at 11.21.18 AM.png" alt=""><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/Screenshot 2025-12-31 at 11.24.20 AM.png" alt=""><figcaption></figcaption></figure></div>

## Creating a command

I recommend looking at the `examples.yml` document and the [documentation](https://dev.bukkit.org/projects/mycommand/pages/configuration-and-example) to look at the possibilities. You can either open an already-made YAML document or create your own .yml

{% hint style="warning" %}
If a command is showing up red, add the following to the command

```yaml
register: true
```
{% endhint %}

### Alias

An alias is the most basic command you can make. It's a way to run an already-made function with a different command. e.g.

This will mean people can run `/gm` to change gamemode if they have permission to run that command

```yml
gamemode_alias:
  command: /gm
  type: ALIAS
  alias: /gamemode
  permission-required: true
```

{% hint style="info" %}
If you wish to create multiple aliases for one command, you'll have to create multiple commands
{% endhint %}

{% hint style="success" %}
Save and run `/mycmd-reload commands` . If it doesn't work, check logs for errors.
{% endhint %}
