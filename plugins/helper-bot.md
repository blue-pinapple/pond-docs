---
description: Automated Bot that replies to your questions
---

# Helper Bot

Locate `/default/plugins/HelperBot`

Questions are created using regex. You can use [https://regex101.com](https://regex101.com) to test. Adding `(?i)` makes it non-case-sensitive

```yml
questions:
  -
    question: '(?i)How (i|to) spawn' #This in regex
    answer: Try /spawn
    # Cooldown is in seconds
    cooldown: 5
    # If broadcast is true, the cooldown is global, if not, its per-player
    # Broadcast true = all players see the bot answer.
    broadcast: yes
    # You can add this on any question to disable it without removing it from the file.
    # disable: yes
    # Whether to show the question message or not (user message).
    broadcast_question: yes
```



you can run `/helperbot setname &e[&6Bot&e] &fGoose &f»&7` to change it's name
