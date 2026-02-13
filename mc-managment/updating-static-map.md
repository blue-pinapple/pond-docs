---
icon: map
---

# Updating Static Map

{% hint style="info" %}
Videos on this page are examples from another server, the files and setup may be different.
{% endhint %}

### Pre-requisets

* Download [Github desktop](https://desktop.github.com/download/) and clone the repo: `https://github.com/blue-pinapple/The-Pond-Rendered-map`&#x20;
* Download [uNmINed](https://unmined.net/)
* Add the following presets into the unmined preset folder (watch clip)

{% columns %}
{% column %}
{% file src="../.gitbook/assets/plots75.json" %}
{% endcolumn %}

{% column %}
{% file src="../.gitbook/assets/plots251.json" %}
{% endcolumn %}

{% column %}
{% file src="../.gitbook/assets/SMP_Nether_2.json" %}
{% endcolumn %}

{% column %}
{% file src="../.gitbook/assets/Overworld.json" %}
{% endcolumn %}
{% endcolumns %}

{% file src="../.gitbook/assets/Screen Recording 2024-10-27 at 10.40.10 am.mov" %}

### **Update Map Instructions**

Complete these each time you want to update

{% stepper %}
{% step %}
### Download world


{% endstep %}

{% step %}
### Press "Fetch Origin" \[GitHub Desktop]

This insures that any changes someone else has made are synced with yours
{% endstep %}

{% step %}
### Locate level.dat or register folder \[uNmINed]

If you always save the world in the same location, I recommend registering the `default` directory, then double-clicking on the level.dat in the left explorer.

<figure><img src="../.gitbook/assets/Screenshot 2026-02-14 at 12.18.05 PM.png" alt="" width="269"><figcaption><p>Left is locate level.dat and right is register</p></figcaption></figure>
{% endstep %}

{% step %}
### Set Preset

Head to the preset tab (on the right) and press <i class="fa-play">:play:</i> on the relevant preset&#x20;
{% endstep %}

{% step %}
### Export

Locate the export tab then select webpage. Change 1:1 to 4:1 and make sure `update changed regions only` is checked. Everything else should be ok at default.

Click the three dots next to output and locate the correct map folder. You can find this folder where you cloned the GitHub repo and it will have the same name as the world. Once this is done, **hit start.**

{% file src="../.gitbook/assets/Screen Recording 2024-10-27 at 10.43.08 am.mov" %}

<figure><img src="../.gitbook/assets/Screenshot 2026-02-14 at 12.32.18 PM.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Repeat

Once it has exported into the folder, repeat steps 3-5 for each world
{% endstep %}

{% step %}
### Commit

Locate the summary box and insert the date of the world download and which worlds you updated. then hit Commit to **main**.

<figure><img src="../.gitbook/assets/Screenshot 2026-02-14 at 12.38.45 PM.png" alt=""><figcaption></figcaption></figure>


{% endstep %}

{% step %}
### Push to Github

Once that is done, click `Repository -> Push` or press ctrl/cmd + P

<figure><img src="../.gitbook/assets/Screenshot 2026-02-14 at 12.40.32 PM.png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
Thats it :) just wait four or so min for the website to update.
{% endhint %}
{% endstep %}
{% endstepper %}

## Update Markers

Locate the `custom.markers.js` in overworld/nether folder to change them. then [#commit](updating-static-map.md#commit "mention") & [#push-to-github](updating-static-map.md#push-to-github "mention")
