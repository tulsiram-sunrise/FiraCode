## Requirements

Make sure you [install the font](https://github.com/tonsky/FiraCode/wiki/Installing).

## Using the Settings Editor

To open the settings editor, first from the `Code` menu choose `Preferences`, `Settings` or use keyboard shortcut <kbd>Ctrl</kbd>+<kbd>,</kbd> (<kbd>Cmd</kbd>+<kbd>,</kbd> on Mac).

To enable FiraCode in the settings editor, under "Commonly Used", expand the "Text Editor" settings and then click on "Font".  In the "Font Family" input box type `Fira Code`, replacing any content.  Tick the check box "Enables/Disables font ligatures" under "Font Ligatures" to enable the special ligatures.

## Manually editing settings.json

Visual Studio Code allows you to also edit the underlying `settings.json` config file.  First open the settings editor as described above, then click the "curly brackets" icon to open the "settings.json" file.

Then paste the following lines and save the file.
```json
"editor.fontFamily": "Fira Code",
"editor.fontLigatures": true,
```

If this doesn't work for you, you can try:
1. restarting VS Code;
1. wrapping the "Fira Code" section with additional apostrophes:
    ```json
    "editor.fontFamily": "'Fira Code'",
    "editor.fontLigatures": true,
    ```
### Font weights
To achieve different weights add one of the following (verified on Mac):
```json
    "editor.fontWeight": "300" // Light
    "editor.fontWeight": "400" // Regular
    "editor.fontWeight": "500" // Medium
    "editor.fontWeight": "600" // Bold
```

To use Retina weight, change Font name to `FiraCode-Retina` if macOS (exactly that, no spaces):
```json
    "editor.fontFamily": "FiraCode-Retina",
```

or 'Fira Code Retina' if Windows or Linux:

```json
    "editor.fontFamily": "Fira Code Retina",
```
