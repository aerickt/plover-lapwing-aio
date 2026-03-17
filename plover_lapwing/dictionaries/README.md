## lapwing-base.json

This dictionary is for Lapwing theory, a free alternative to Plover theory and its `main.json`.

Looking to learn Lapwing theory? Check out the [Lapwing for Beginners Wiki](https://lapwing.aerick.ca).

## lapwing-commands.json
This dictionary contains all main movement, keyboard shortcuts, and Plover commands that I use.

### Dictionary contents

 - [Movement keys](#Movement-keys)
 - [Commands and keyboard shortcuts](#Commands-and-keyboard-shortcuts)

#### Movement keys

By pressing down `STPH` on the left hand, the `-RPBG` cluster becomes arrow keys. `-FR` chorded together would be home, and `-LG` would be end. Pageup and pagedown resemble arrows pointing up and down respectively `-RPG` and `-FBL`.

By pressing `STPH*` instead, the shift modifier is used together with the movement keys in order to select text.

To move word by word (equivalent to pressing `Ctrl+Shift` and left/right), `-RB` and `-BG` are used. On macOS, `Alt+Shift` is used instead so that will have to be changed.

For more details see [Lapwing for Beginners](https://lapwing.aerick.ca/Chapter-26.html).

#### Commands and keyboard shortcuts

Many of the commands from main.json have stayed the same.
 - `KPA` → capitalize the next word
 - `KPA*` → capitalize the next word and supress the next space
 - `HRO*ER` → uncapitalize the next word
 - `TK-LS` → supress the next space

Retroactive commands have also been added.
 - `KA*PD` → capitalize the last word
 - `HRO*ERD` → uncapitalize the last word
 - `TK-FPS` → remove the last space

Common keyboard keys have also carried over from main.json.
 - `R-R` → enter/return (capitalization of next word depends on previous punctuation)
 - `#R-R` → `Shift+Enter`
 - `PW-FP` → backspace one character
 - `PW*FP` → backspace one word (`Ctrl+Backspace`; change to `Alt+Backspace` on macOS)
 - `TKHRE` → delete one character
 - `TKHR*E` → delete one word (`Ctrl+Delete`; change to `Alt+Delete` on macOS)
 - `TA*B` → `Tab`
 - `#TA*B` → `Shift+Tab`

For more details, see [Lapwing for Beginners](https://lapwing.aerick.ca/Chapter-20.html#commands).

For writing every single keyboard shortcut possible, I recommend [Emily's modifiers dictionary](https://github.com/EPLHREU/emily-modifiers).

## lapwing-movement.modal

See also: [semi-modal-movement.json](#semi-modal-movementjson)

This is a modal dictionary that is an extension to the [movement keys in my commands.json dictionary](#Movement-keys).

After the [modal dictionary plugin](https://github.com/Kaoffie/plover_modal_dictionary) has been installed from the plugins manager, ensure Plover has been restarted and the plugin is enabled (configure → plugins). Next add the dictionary above whichever dictionary contains the default movement strokes.

Using this dictionary for movement keys is exactly the same as those in [commands.json](#Movement-keys), however every successive movement stroke after the first does not need to contain the `STPH` cluster.

Examples:
 - `STPH-G/-G/-G/-G` → arrow key to the right 4 times
 - `STPH*R/*R/*R` → select 3 characters to the left
 - `STPH-BG/-BG/-BG` → move to the right by 3 words

## lapwing-numbers.json

A right hand numberpad system. Lapwing not required; can be used with other theories.

See the [Lapwing for Beginners Wiki](https://github.com/aerickt/lapwing-for-beginners/wiki/Chapter-17:-Fingerspelling-and-Numbers#numbers) for more details.

## lapwing-uk-additions.json

A dictionary for UK spellings for use with Lapwing theory. See [Lapwing for Beginners](https://lapwing.aerick.ca/Chapter-20.html) for details.

# Contributing

Changes to the plugin's dictionaries should be applied here.

> Previously the plover-lapwing-aio dictionaries were pulled using git-subrepo from the plover-lapwing-aio branch of my steno-dictionaries repo. This will not be the case moving forward. I am treating the steno-dictionaries repo as a collection of my personal dictionaries, while the official Lapwing dictionaries will reside here.

