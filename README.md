# Plover Lapwing AIO

[![pypi](https://img.shields.io/pypi/v/plover-lapwing-aio)](https://pypi.org/project/plover-lapwing-aio/) [![pypi](https://img.shields.io/pypi/dm/plover-lapwing-aio.svg)](https://pypi.org/project/plover-lapwing-aio/) [![paypal](https://img.shields.io/badge/-Buy%20me%20a%20coffee%20%3AD-informational?logo=paypal)](https://www.paypal.com/donate/?hosted_button_id=VNMUULBPTQGMC)

Lapwing AIO automatically installs all the necessary plugins and dictionaries for using Lapwing theory with Plover.

## Installation

In Plover's main window, click on `Tools → Plugins Manager`. Scroll down until you see `plover-lapwing-aio` and select it. Press the `Install/Update` plugin and make sure to press `Restart` afterwards.

![plugins manager](https://lapwing.aerick.ca/img/5-plugins-manager.png)

> NOTE: just closing the main window is not sufficient to restart Plover. **You will have to press the restart button or manually quit Plover by going to `File → Quit Plover` and opening Plover again.**

Once Plover has been restarted, in Plover's main window, click on `Configure → System` and change the system to `Lapwing`. Press `Apply` and `OK`—you should now be good to go!

![system settings](https://lapwing.aerick.ca/img/5-system.png)

## Usage

Under Plover's configuration, change the system to "Lapwing" under the system tab. Note that your dictionary stack will be reset and you will have to re-add any dictionaries you've previously used.

For modal movement to work, you will also have to enable the modal dictionary extension. Go to `Configure → Plugins` and check the  `modal_update` box. Please note that this plugin is somewhat hacky and may cause issues with other plugins such as plover-clippy2 and plover-tapey-tape when enabled.

### How to learn Lapwing

Check out the [Lapwing for Beginners](https://github.com/aerickt/lapwing-for-beginners/wiki) wiki!

## Features

### Dictionaries

This plugin adds the following dictionaries by default:

- user.json
   - This is the same dictionary used in the default English stenotype system
   - If you have made additions to this dictionary, they will carry over to Lapwing
- [jeff-phrasing.py](https://github.com/jthlim/jeff-phrasing)
   - Comprehensive phrasing system with automatic conjugation
- [abby-left-hand-modifiers.py](https://github.com/Abkwreu/plover-left-hand-modifiers)
   - Python dictionary for one-hand shortcuts
- [emily-modifiers.py](https://github.com/EPLHREU/emily-modifiers)
   - Python dictionary for two-handed shortcuts
- [emily-symbols.py](https://github.com/EPLHREU/emily-symbols)
   - Python dictionary for systematic symbols
- [lapwing-movement.modal](https://github.com/aerickt/steno-dictionaries/blob/plover-lapwing-aio/lapwing-movement.modal)
   - Modal dictionary for easy movement
   - See [chapter 26](https://github.com/aerickt/lapwing-for-beginners/wiki/Chapter-26:-Editing-Text) of the Lapwing wiki for more details
- [lapwing-commands.json](https://github.com/aerickt/steno-dictionaries/blob/plover-lapwing-aio/lapwing-commands.json)
   - Plover commands and common shortcuts
- [lapwing-numbers.json](https://github.com/aerickt/steno-dictionaries/blob/plover-lapwing-aio/lapwing-numbers.json)
   - Right hand numberpad system
- [lapwing-uk-additions.json](https://github.com/aerickt/steno-dictionaries/blob/plover-lapwing-aio/lapwing-uk-additions.json)
   - UK spellings
- [lapwing-proper-nouns.json](https://github.com/aerickt/steno-dictionaries/blob/plover-lapwing-aio/lapwing-proper-nouns.json)
   - Proper nouns
- [lapwing-base.json](https://github.com/aerickt/steno-dictionaries/blob/plover-lapwing-aio/lapwing-base.json)
   - Main Lapwing dictionary

### Plugins

The following plugins are included when you install plover-lapwing-aio:

 - plover-dict-commands
 - plover-last-translation
 - plover-modal-dictionary
 - plover-python-dictionary
 - plover-stitching

### Number key behaviour

With stock Plover, pressing the number key shifts several keys into numbers. Using the lookup tool, any entries with the number key in it would show up with numbers in the outline. However, with this plugin, the number key is simply just another key. In steno order, it is at the very beginning. This makes it much easier to read and add outlines with the number key.

### Top `S` number key relocation

This plugin contains several keymaps which automatically remaps the top `S` key to the number key.
