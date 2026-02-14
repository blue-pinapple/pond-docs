---
description: >-
  How to edit the components/Questions of the discord forms i.e Pond
  application.
icon: wpforms
---

# Editing Form Components

Editing the form is a pain, but this is how you do it. A component is a section/question of the form.

{% stepper %}
{% step %}
### Preperation

Before you start, I recommend opening the form and copying what it currently is
{% endstep %}

{% step %}
### /edit & selecting the form

Running `/edit` will bring up a dropdown. Select the form you wish to edit.

{% hint style="info" %}
You will have to run this for each change
{% endhint %}

<div><figure><img src=".gitbook/assets/Screenshot 2026-01-09 at 5.02.12 PM.png" alt=""><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/Screenshot 2026-01-09 at 5.03.24 PM.png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Adding Component&#x20;

On the next dropdown, select the option to add a component (question). Then proceed to fill out the form. Once you are done, this will add the question at the **end of the form.**

<div><figure><img src=".gitbook/assets/Screenshot 2026-01-09 at 5.03.41 PM.png" alt=""><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/Screenshot 2026-01-09 at 5.06.35 PM.png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Removing Old Component

To prevent double questions, we must remove the old one. Run `/edit` like in [Step 2](editing-form-components.md#edit-and-selecting-the-form)

<div><figure><img src=".gitbook/assets/Screenshot 2026-01-09 at 5.07.01 PM.png" alt=""><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/Screenshot 2026-01-09 at 5.13.50 PM.png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Verify

Any form button should update without needing to run `/send`. I recommend checking that the form is how you want before continuing.
{% endstep %}

{% step %}
### Sending (Optional)

If you do end up needing to send it again, use `/send` and select the right forms.

Here is an example:

```
/send channel:<#1282813983635804210> title:Server Application description:Press the button bellow to get whitelisted on the MC server. I still recomend reading the above. color:Orange
```
{% endstep %}
{% endstepper %}


# Actions
To edit an action, create a new one then delete the old. `/action ...`
## Send Channel Example
```
{user}
**{question-1}**
{value-1}
**{question-2}**
{value-2}
**{question-3}**
{value-3}
**{question-4}**
{value-4}
```
```
<@&1260740257499058250> Check https://pond-docs.gitbook.io/mods/mc-managment/bedrock-geyser for linking & alt. 
https://pond-docs.gitbook.io/mods/mc-managment/transferring-accounts for transfer.
```
