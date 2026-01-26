---
description: How the restore chunk plugin works
---

# Restore Chunk

The following is taken from the [Github README](https://github.com/Warriorrrr/RestoreChunk/)

&#x20;<a href="restore-chunk.md#how-to-restore-a-chunk" class="button primary" data-icon="forward">Skip to guide</a>



### Usage

The main command used by the plugin is /restorechunk. To start, you first need to place the region file you want to restore from in the `/plugins/RestoreChunk/$world$/region` directory. You will then be able to use the command to restore the current chunk you're standing in.

#### Custom arguments

Custom arguments can be used with the restorechunk command to fine tune which blocks get restored.

**`i:`/`include:`**

Limits restored blocks to the given blocks.

Example: `/restorechunk include:dirt,stone` will only restore any missing dirt or stone in the chunk.

**`p:`/`predicate:`**

Allows you to use the blocks x, y, or z coordinate as a factor for whether it gets restored or not.

Example: `/restorechunk p:y>70` will only restore blocks above y level 70.

| Operator | Description           |
| -------- | --------------------- |
| >        | Greater than          |
| <        | Lesser than           |
| >=       | Greater than or equal |
| <=       | Lesser than or equal  |
| =        | Equals                |
| %        | Remainder (true if 0) |
| &        | Bit mask (true if 0)  |

**`#preview`**

Allows you to preview the changes without altering the world. You can use `/restorechunk apply` to apply the changes you're previewing. There is currently no way to cancel a preview, other than walking away until the chunk is out of view distance.

**`#relight`**

Relights all adjacent chunks, useful if there are lightning issues at the chunk edge.

### Permissions

There is currently only the `restorechunk.command.restorechunk` permission, used for the main command and given to operators by default.

## How to restore a chunk

This will show you how to restore a chunk from a backup that is in a zip format.

{% stepper %}
{% step %}
### Prep: Clear old data

We must first check that the restore chunk folder is clear so we can restore the new stuff. The folder is located at `/default/plugins/RestoreChunk`  &#x20;

<figure><img src="../.gitbook/assets/Screenshot 2026-01-22 at 6.11.02 PM.png" alt=""><figcaption></figcaption></figure>


{% endstep %}

{% step %}
### Move zip into the default folder

Locate the backup zip file that you may need in `/default/backups/{world}/` and drag it into the default folder. We do this so we can easily move/extract it to subfolders of default

<div><figure><img src="../.gitbook/assets/a1c9217932cc16c3f443bb68f7fe83e6.png" alt=""><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/ca8782dec3142b505bac2f34ac5cd08e copy (1).jpg" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Extract into RestoreChunkk folder

<div><figure><img src="../.gitbook/assets/33ee77a1c041af7fbd53513868266645.png" alt=""><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/8a0c6d04dea86913400c6f50a2f1d679.png" alt=""><figcaption></figcaption></figure></div>

Right-click on the zip -> click `Extract to folder` . Then replace the default folder path with `plugins/RestoreChunk/{world}` .The RestoreChunk folder should appear siliar to bellow

<figure><img src="../.gitbook/assets/fdf5ea272dad90170fdc78090c7d054c.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Move Zip Back

Move the zip back to it's origonal folder, this can be done by right clicking -> `Rename` then changing it to `backups/{world}/{name}` &#x20;

<figure><img src="../.gitbook/assets/069f6407c7a4358f4bf5e78425374bda.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Restore the chunk

On the server, locate the chunk you wish to restore (f3 + g to view chunk borders) and run `/restorechunk` You should see it correctly restored.

<div><figure><img src="../.gitbook/assets/Screenshot 2026-01-22 at 6.10.02 PM (1).png" alt=""><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/Screenshot 2026-01-22 at 6.10.09 PM.png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Reset RestoreChunk Folder

Clear the folder, like in step 1
{% endstep %}
{% endstepper %}
