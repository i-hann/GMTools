# Roll20 GMTools
## Overview
GMTools.js is a script that can be loaded into Roll20 to automate various tasks that a GM must often perform when running a game of Pathfinder 2, as well as enrich the game with additional features.


## Features
Use the !reset command in chat to create all of the macros used by this script. This will also delete existing macros with the same names.

### Debug (Macro - Token Action)
Displays Id, Type, Subtype, Pageid, Controlledby, and Tint_color of the selected token. Only works if a single token is selected.

### Reset-Sfx (Macro)
Refreshes the active playlist of Death sound effects, allowing you to delete or add them during the game without needing to reload the script.

### Group-Initiative (Macro - Token Action)
Rolls Initiative for the selected token(s), displaying the results in chat and adding each token to the turn order. Assumes each token to have "Bar1_Value" set to it's Initiative modifier.

### Group-Saves (Macro - Token Action)
Rolls Saving Throws for the selected token(s). Tokens with the same image are assumed to have the same Saving Throw modifiers. On execution, the command first queries the GM for the Saving Throw type (Fortitude, Reflex, or Will) and the DC (ex: 17). Then a chat menu is displayed with a "ROLL" button for each Token Group. Pressing a ROLL button queries the GM for the Saving Throw modifier of that Token Group. Then, it rolls all of the saves for the group and displays them in a new table with custom HTML.

### Death Sound Effects
Treating Bar 3 as HP, any token that drops to 0 HP or lower will trigger a Death sound effect from the Roll20 Jukebox. In order for a Jukebox item to be used as a Death sound effect, it's title needs to begin with "Death:" (ex: "Death: Wilhelm Scream").

