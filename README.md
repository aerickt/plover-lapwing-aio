# Plover Lapwing AIO

[![pypi](https://img.shields.io/pypi/v/plover-lapwing-aio)](https://pypi.org/project/plover-lapwing-aio/)

Lapwing AIO automatically installs all the necessary plugins and dictionaries for using Lapwing theory with Plover.

## Installation

~~plugins manager~~ (WIP)

## Usage

Under Plover's configuration, change the system to "Lapwing Stenotype" under the system tab. Note that your dictionary stack will be reset and you will have to re-add any dictionaries you've previously used.

For modal movement to work, you will also have to enable the modal dictionary extension. In Plover's configuration, go to the plugins tab and check modal dictionary box. Please note that this plugin is somewhat hacky and is incompatible with other plugins such as plover-clippy2 and plover-tapey-tape.

### How to learn Lapwing

Check out the [Lapwing for Beginners](https://github.com/aerickt/lapwing-for-beginners/wiki) wiki!

## Features

### Dictionaries

This plugin adds the following dictionaries by default:

- user.json
   - This is the same dictionary used in the default English stenotype system
   - If you have made additions to this dictionary, they will carry over to Lapwing
- movement.modal
   - Modal dictionary for easy movement
   - See [chapter 26](https://github.com/aerickt/lapwing-for-beginners/wiki/Chapter-26:-Editing-Text) of the Lapwing wiki for more details
- [jeff-phrasing.py](https://github.com/jthlim/jeff-phrasing)
   - Comprehensive phrasing system with automatic conjugation
- [abby-left-hand-modifiers.py](https://github.com/Abkwreu/plover-left-hand-modifiers)
   - Python dictionary for one-hand shortcuts
- [emily-modifiers.py](https://github.com/EPLHREU/emily-modifiers)
   - Python dictionary for two-handed shortcuts
- [emily-symbols.py](https://github.com/EPLHREU/emily-symbols)
   - Python dictionary for systematic symbols
- [lapwing-uk-additions.json](https://github.com/aerickt/lapwing-for-beginners/wiki)
   - Lapwing dictionary for UK spellings
- [lapwing-base.json](https://github.com/aerickt/lapwing-for-beginners/wiki/Chapter-20:-UK-Spellings)
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