# Dreamlight Editor

A clean and safety-minded Windows editor for Disney Dreamlight Valley save files.

Dreamlight Editor focuses on careful save editing, readable JSON tools, automatic backups, and a calm interface that helps you understand what you are changing before you save.

## ✨ Features

- Load and decrypt Disney Dreamlight Valley save files.
- Edit supported save sections through organized tables.
- Save edited data back to the selected profile file.
- Full JSON Editor for direct save inspection and advanced manual edits.
- Export the decrypted save as a readable JSON file.
- Import a decrypted JSON file back into the editor.
- Validate and format JSON before saving or importing.
- Automatic backup creation before important file operations.
- Compact save writing, so edited files are not artificially expanded.
- Search and filter support across editor grids.
- Sortable table columns for easier browsing.
- Multi-select editing for supported grid values.
- Status labels for the loaded save version, player name, level, and editor state.
- Modern themed interface with improved readability.

## 🛡️ Safety First

Save editing is never completely risk-free, so the editor includes several safeguards:

- A backup is created before save files are decrypted or imported.
- JSON imports are checked before they are accepted.
- Invalid JSON is blocked and reported with line and column information.
- The Full JSON Editor validates the save structure before writing changes.
- Save data is written in a compact format to avoid unnecessary file bloat.
- Existing item metadata is preserved where supported instead of replacing entries with minimal data.
- Clear error messages are shown when a file cannot be loaded, parsed, or saved.

Even with these safeguards, always keep your own backup before testing edited saves in game.

## 🧾 JSON Export / Import

The Full JSON Editor includes tools for working with decrypted JSON:

- **Export Decrypted JSON** creates a readable JSON copy that can be inspected or edited outside the app.
- **Import Decrypted JSON** lets you load a modified JSON file back into the editor.
- Imported JSON must be valid and must contain the expected save structure.
- A backup is created before an imported JSON file is accepted into the editor workflow.

This is useful for careful manual edits, comparing changes, or keeping an extra readable copy of a save.

## 🖥️ Editor / Interface

The editor provides a structured interface for common save sections, including:

- Player inventory
- Pets
- Clothes
- Houses
- Furniture
- Makeup
- Skins
- Mounts
- Mount gear
- Gliders
- Avatar features
- Tools and accessories

The Full JSON Editor includes:

- Dark editor view
- JSON syntax highlighting
- Line numbers
- Current line, column, character count, and modified status
- Format JSON
- Validate JSON
- Search
- Copy
- Undo and redo

## 📦 Download

1. Open the latest release on this repository's **Releases** page.
2. Download the ZIP file.
3. Extract the ZIP completely.
4. Start the editor from the extracted folder.

Do not run the editor directly from inside the ZIP file. Some required files need to stay next to the executable.

## 🚀 How to Use

1. Start Dreamlight Editor.
2. Choose or load your save file.
3. Let the editor create its backup before making changes.
4. Edit the supported sections you want to change.
5. Optionally open the Full JSON Editor for advanced inspection or JSON export/import.
6. Save your changes.
7. Start the game and test the edited save carefully.

## ⚠️ Important Notes

- Always keep a separate backup of your original save.
- Test small changes first.
- Avoid making many risky changes at the same time.
- If something looks wrong in game, restore a backup instead of continuing from the edited save.
- Savegame editing can break progression or game data if used carelessly.

## 🧪 Recommended Testing

After editing a save, check the basics in game:

- The game starts normally.
- The save loads successfully.
- Player inventory opens correctly.
- The map opens correctly.
- Quests still appear normal.
- Edited values or items are visible where expected.
- No error messages appear while loading or playing.

## 🧰 Troubleshooting

- Restore your latest backup if the game does not load the edited save.
- Revert the last change and test again.
- Use the Full JSON Editor's validation tool if you edited JSON manually.
- Make smaller changes and save again.
- If an imported JSON file is rejected, check that it is valid JSON and still contains the expected save structure.
- Make sure the ZIP was fully extracted before starting the editor.

## 💙 Disclaimer

This is an unofficial fan-made tool and is not affiliated with Disney, Gameloft, or Disney Dreamlight Valley.
