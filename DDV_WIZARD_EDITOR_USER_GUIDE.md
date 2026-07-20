# DDV Wizard Editor – User Guide

This guide explains how to use the public DDV Wizard Editor. It covers opening, editing, checking, and restoring save files in version **0.9.7**.

The guide is written for version **0.9.7**. Menu names may move slightly in later versions, but the safety rules remain the same.

## Contents

1. Before you start
2. Downloading and opening the editor
3. Sign-in and activation
4. Automatic editor-data updates
5. Opening the correct save
6. Automatic and manual backups
7. Understanding the main window
8. Search and expansion filters
9. Adding, removing, and editing items
10. Category guide
11. Inventory Categories and bulk actions
12. Pavings and Fencing
13. Inventory Size Fix
14. Evolving tools and wings
15. Manage House Floors
16. Fixes and repair tools
17. Missing, unknown, blocked, and misplaced items
18. Full JSON Editor
19. Saving and validating a save
20. Common warnings and errors
21. Safety rules

## 1. Before you start

The editor changes a real game save. Most normal edits are straightforward, but a wrong item, an extreme value, or a damaged JSON structure can prevent the game from loading correctly.

Before every editing session:

- Close Disney Dreamlight Valley completely.
- Confirm that you are using the newest official editor release.
- Extract the complete ZIP into its own folder.
- Keep all files from the ZIP together.
- Keep a separate copy of the original profile.json.
- Test a small number of changes before making a large batch.

Never combine the executable, Dict files, or protected data from different editor versions.

## 2. Downloading and opening the editor

The editor is portable and does not need to be installed.

1. Download the newest ZIP from the official Releases page.
2. Extract the complete ZIP into a new folder.
3. Open **Dreamlight Editor - Public.exe**.
4. Leave the other included files beside the executable.

Do not start the editor directly from inside the ZIP. If Windows reports that a runtime is missing, install the free **Microsoft .NET 8 Desktop Runtime (x64)**.

The title bar displays the editor version and build. Include both when reporting a problem.

## 3. Sign-in and activation

The public editor requires an email sign-in.

1. Enter an email address you can access.
2. Select **Send code**.
3. Enter the six-digit code sent to that inbox.
4. Select **Sign in**.

The sign-in is normally remembered on that computer. A new code should not be required every time the editor starts.

A normal activation is intended for one Windows computer and can be connected to up to three different save profiles. Reinstalling the editor or downloading a newer build does not intentionally reset that profile limit.

The sign-in requirement exists because a small number of people used the free editor to make money from other players. It helps limit that misuse while keeping normal community access simple.

### Sign-in problems

- **The code is invalid or expired:** request a new code and use the newest email.
- **The email is slow:** wait a moment and check the spam folder before requesting several more codes.
- **Too many attempts:** stop retrying and wait before trying again.
- **This computer is already registered:** use the original email or contact support.
- **Maximum profiles reached:** one of the registered profiles must be reviewed or released by support.
- **Activation blocked or manual review required:** contact support rather than repeatedly registering new details.
- **Editor version no longer authorized:** download the newest official release.
- **Protected editor data could not be unlocked:** connect to the internet and restart the editor.

## 4. Automatic editor-data updates

The editor can receive updated item lists and corrections without requiring a completely new download.

- Updates are checked during startup.
- The downloaded editor data is protected and verified before use.
- A message named **Editor Data Updated** appears when a new update was installed successfully.
- If an update is unavailable or damaged, the editor falls back to a valid cached or built-in copy where possible.

An editor-data update can add names, IDs, expansion assignments, or corrections. It cannot replace program features that require a new executable, so full editor releases are still needed for larger changes.

## 5. Opening the correct save

Use **Tools > Load Save** and select the file named **profile.json**.

The usual Windows location is inside:

**AppData > LocalLow > Gameloft > Disney Dreamlight Valley**

Different platforms or accounts may have several save folders. After loading, always check the player name and level displayed at the top of the editor. If they do not match the intended player, stop and choose the correct profile.

Use **Tools > Change Save Location** when you want to switch to a different profile.json. The selected location is remembered for future starts.

The editor must load the save successfully before category tabs, saving, currencies, and most Tools actions become available.

## 6. Automatic and manual backups

### Automatic backups

The editor creates safety copies during important load, import, delete, and repair operations.

Two useful backup locations may be used:

- A time-stamped backup beside the selected profile.json.
- A rolling backup set under **Documents > Dreamlight Valley Editor > Backups**.

The rolling backup folder keeps the original safety copy and a limited number of newer backups for the same save location.

Some focused tools, such as House Floor management, Collection repair, and deletion from All Save Items, create their own backup before changing the save.

### Manual backup

There is no reason to rely on only one automatic backup.

1. Close the game.
2. Copy the original profile.json to a separate folder.
3. Rename the copy clearly, for example **profile_before_editor_2026-07-20.json**.
4. Do not edit that manual copy.

### Restoring a backup

1. Close the game and editor.
2. Keep a copy of the broken save for investigation.
3. Copy the chosen backup into the real save folder.
4. Rename it to **profile.json** if needed.
5. Start the game before making more editor changes.

Do not post a profile.json publicly. If support needs the file, use a private support channel.

## 7. Understanding the main window

The top area shows:

- **Editor version and build** in the title bar.
- **Player name and level** after loading a save.
- **Status**, such as Ready, Loaded, Saved, Error, or Activation required.
- **Role label** when a role is assigned.
- **Search** for filtering the current category.
- **Expansion** for filtering visible content by game or DLC.
- **Tools** for loading, saving, bulk actions, fixes, and advanced utilities.

Each main tab includes a count. The count reflects the rows currently available in that category and can change after loading, filtering, adding, or removing entries.

## 8. Search and expansion filters

### Search

Search filters the currently visible grid. Depending on the category, it can match names, IDs, or other displayed fields.

Search does not remove anything from the save. Clear the search field to show the full current category again.

### Expansion filter

The Expansion menu applies across supported categories:

- All content
- Base Game
- Eternity Isle
- Storybook Vale
- Wishblossom Ranch
- Honeyglow Woods

This is only a display filter. Choosing an expansion does not add, delete, lock, or change ownership of any item.

Expansion detection uses the current editor data. If an item appears under the wrong expansion or is not found, return to **All content** and search by item ID.

## 9. Adding, removing, and editing items

Most category grids use a right-click menu.

Common actions include:

- **Add Item** – enter an item ID and, where supported, an amount.
- **Delete** – remove the selected row or rows.
- **Change Selected Values / Amount** – apply one value to all selected rows.
- **Unlock in Collection** – mark supported selected items as visible in the Collection.
- **Delete From Collection** – remove the Collection unlock without necessarily removing the owned item.

You can select several rows before right-clicking. Right-clicking a selected row keeps the full selection where that action supports multiple items.

### Important difference: ownership and Collection

An item stored in an inventory and an item marked as unlocked in the Collection are not always the same thing.

- Adding an item changes ownership or inventory data.
- Unlocking in Collection changes Collection visibility.
- Removing from Collection does not automatically delete the owned item.
- Collection repair only reconnects supported Collection entries for items the save already owns.

Use the action that matches the actual problem.

### Protected or excluded entries

Some entries are visible but cannot be added, deleted, or changed. They may be required by the game, linked to progression, unsafe, or intentionally excluded. A skipped protected entry is a safety feature, not an editor failure.

## 10. Category guide

### Pets / Companions

The Pets tab shows companions stored in the save.

You can:

- add an individual supported companion;
- remove selected companions;
- change supported values;
- unlock selected companions in the Collection;
- show missing companions and add selected missing pets to the save;
- use **Inventory Categories > Pets** for supported Add All or Collection actions.

Do not assume that every internal or quest companion is safe to add.

### Clothes

The Clothes tab contains wearable inventory entries.

You can:

- add or remove individual clothes;
- change selected amounts where supported;
- unlock or remove selected Collection entries;
- add all supported clothes;
- unlock all supported clothes in the Collection.

Quest, mission, temporary, or placeholder clothing should not be added casually.

### Houses and Buildings

The Houses tab separates entries into:

- All
- Villagers Houses
- Players Houses
- Stall
- Other Buildings

These groups help identify the purpose of an entry. They do not change the order used by the game.

You can add or remove supported house and building entries. **Inventory Categories > Add All Houses** adds the supported safe list, not every internal building ID known to the game.

Use **Tools > Manage House Floors** for room and floor removal. Do not try to remove house floors by deleting random JSON sections.

### Furniture

The Furniture tab includes normal furniture and separate views for Pavings and Fencing.

You can:

- add or remove individual entries;
- change selected amounts;
- unlock or remove selected Collection entries;
- add all supported furniture without known bug items;
- unlock supported furniture in the Collection;
- add Pavings, Fencing, or both with a chosen amount.

Large furniture batches can make a save harder to review. Add only what is needed whenever possible.

### Player Inventory

The Player Inventory tab shows items stored in the player backpack or related player inventory section.

You can add, remove, or change supported amounts. Be careful with quest objects, currencies represented as items, progression objects, and unknown IDs.

Inventory capacity is handled separately through **Fix Inventory Space**.

### Makeup

The Makeup tab allows supported makeup entries to be added, removed, or edited. **Inventory Categories > Add All Makeup** adds the current supported list.

### Skins

The Skins area separates:

- All
- NPC skins
- Wells
- Goofy Stalls
- Other building skins

You can add or remove supported skins and use the Tools menu to add all supported NPC or building skins. Protected skins are intentionally skipped.

### Mounts

The Mounts tab manages supported mount ownership and Collection state.

You can add or remove individual mounts, change supported values, and use the category menu to add all supported mounts or unlock them in Collection.

### Mount Gear

The Mount Gear tab contains supported equipment or appearances connected to mounts. It supports individual add, delete, and value changes, plus the supported Add All action.

### Gliders

The Gliders tab contains ground gliders and other supported glider entries.

Wing-style gliders normally belong in Clothes, while ground gliders belong in the Gliders inventory. If the same glider appears repeatedly or wings are stored incorrectly, use **Tools > Fixes > Fix Duplicate Gliders**.

### Avatar Features

The Avatar Features tab includes supported avatar features and eyeball entries.

Available actions include:

- add a feature by ID;
- delete a supported selected feature;
- change selected amounts;
- repair missing eyeballs from the current Dict.

Protected entries may be skipped.

### Tools / Accessories

This area separates normal Tools from Accessories.

Use individual add or delete actions only for known supported IDs. **Inventory Categories > Add All Tools (Safe to Use)** uses the protected safe list.

Evolving tools require more than one visible tool item. Use the Evolving actions described later instead of manually adding only the final variant.

### Wallpaper and Flooring

The Wallpaper and Flooring tab allows individual supported walls and floors to be added or removed.

Use this tab when only a few entries are needed. **Inventory Categories > Add All Wallpapers and Floors** adds the supported bulk list.

Entries already present in the save remain visible even when they are no longer normally offered for adding, allowing an incorrect entry to be identified and removed.

### Meals

The Meals tab represents recipe Collection progress, not a backpack full of cooked meals.

- Change the **Unlocked** box for an individual supported recipe.
- Use **Inventory Categories > Unlock All Meals in Collection** for the supported bulk list.
- Excluded or protected meal entries remain unavailable.

### Memories

The Memories tab shows supported memory progress.

You can unlock or remove individual supported memories. Story, quest, removed, or protected definitions receive additional warnings or cannot be edited.

Under **Tools > Memories**:

- **Add All** unlocks supported safe event and non-story memories.
- **Add Memory Mania (Achievements and Rewards)** adds missing Memory Mania progress and rewards without replacing unrelated save data.

Do not force story or quest memories simply to complete the Collection screen.

### Touch of Magic Decals

**Inventory Categories > Add All Touch of Magic Decals** adds the current supported decal list. This is a bulk action; keep a backup and verify the result in game.

### Currencies

After loading a save, **Tools > Currencies** lists editable supported currencies and their current values.

Select a currency to change it. Use reasonable values and avoid currencies that are not shown by the editor.

Pixel Dust is intentionally excluded because editing or adding it can risk account flagging or other unwanted consequences.

## 11. Inventory Categories and bulk actions

The **Tools > Inventory Categories** menu contains bulk actions for supported content, including:

- Pets and companion Collection
- Clothes and clothing Collection
- Furniture and furniture Collection
- Pavings and Fencing
- NPC and building skins
- Houses
- Mounts and Mount Gear
- Makeup
- Wallpapers and Floors
- Touch of Magic decals
- Safe tools
- Gliders
- Meals Collection
- Missing Dict items
- All Save Items, including unknown entries

Bulk actions are convenient but harder to review than individual changes.

Recommended approach:

1. Create a manual backup.
2. Run one bulk action.
3. Read the status message.
4. Save if the action is pending.
5. Test the save in game before running another large action.

Some Tools actions write to the save immediately after confirmation. Do not assume that closing the editor will cancel every bulk or repair action.

## 12. Pavings and Fencing

The interface uses the wording **Pavings and Fencing** for paths and fences.

Available actions:

- Add All Pavings
- Add All Fencing
- Add All Pavings and Fencing

The editor asks for the amount to add. The chosen amount is applied to the supported entries in that action.

Use a sensible amount. Extremely large stacks are unnecessary, can make inventories difficult to inspect, and may create unexpected in-game behavior.

Pavings and Fencing are also visible as Furniture subcategories for individual review.

## 13. Inventory Size Fix

Use **Tools > Fix Inventory Space** only for the player backpack.

Available sizes:

- **Initial without Upgrade (21)** – returns the backpack to the initial size.
- **Default (42)** – returns it to the standard upgraded size.
- **Expanded Backpack (84)** – enables the larger supported backpack layout.

The fix does not change companion inventory slots.

Before switching to 42, remove equipped companions if the editor warning asks you to do so. After choosing 84, sort the backpack once in game. If items remain hidden, move visible items to a chest and sort again.

Never reduce inventory size while valuable items may be stored in slots that will disappear. Move items out first and keep a backup.

## 14. Evolving tools and wings

Use **Tools > Evolving**.

### Tools to Level 3

This action adds the supported Evolving Watering Can, Pickaxe, and Fishing Rod data together with:

- the required tool variants;
- the Level 2 and Level 3 item IDs;
- completed supported progression entries.

### Elegant Firework Wings to Level 3

This adds the supported wings and completes their supported progression.

Do not manually add only a Level 3 tool variant. The game checks both the owned variants and the Evolve progress. An incomplete manual edit can make the tool disappear or become unusable.

## 15. Manage House Floors

Open **Tools > Manage House Floors** after loading a save.

The tool lets you select a player house and:

- clear the first floor without deleting the required first-floor structure;
- remove selected higher floors;
- return furniture placed on removed floors to the Furniture inventory.

The tool shows a confirmation and creates a backup beside the save.

Check the selected house and floor numbers carefully. Removing a floor is much broader than deleting one furniture item.

## 16. Fixes and repair tools

Open **Tools > Fixes**.

### Fix Duplicate Gliders

Use this when gliders are duplicated or stored in the wrong inventory.

The repair:

- removes duplicate glider data;
- returns wing gliders to Clothes;
- keeps ground gliders in the Gliders inventory.

### Repair Collection From Owned Items (Beta)

Use this when the save owns items but the Collection does not recognise them, or when completed Collection groups contain contradictory locked entries.

The repair:

- unlocks supported Collection entries for item IDs the save actually owns;
- corrects contradictory group states;
- respects explicitly excluded IDs;
- does not add inventory items;
- does not invent new Collection IDs;
- creates a backup and a report when changes are needed.

This is a repair tool, not an Add All function. Do not use it to obtain items the save does not own.

## 17. Missing, unknown, blocked, and misplaced items

### Show Missing Dict Items

Open **Tools > Inventory Categories > Show Missing Dict Items**.

This displays supported editor items that are not currently present in the loaded save.

- It does not automatically add everything.
- Amount-based entries appear with amount 0 until deliberately changed.
- Missing pets must be selected and added to the save through their right-click action.
- The entries appear in their normal category tabs for review.

Use this mode when you want to find a specific missing supported item instead of using Add All.

### Items already present in a save

Items found in the loaded save remain visible in their matching category even if they are:

- unknown to the current name list;
- no longer normally offered;
- blocked from being added again;
- excluded from bulk actions.

This makes it possible to identify and remove a bad entry without allowing another copy to be added.

### All Save Items (including unknown) – Beta!

Open **Tools > Inventory Categories > All Save Items (including unknown) - Beta!**

This window searches all Player inventory entries and shows:

- Item ID
- Name when known
- Amount
- Storage location
- Status

Use the search field to find an ID, name, storage section, or status.

Deletion from this window is immediate. It creates a backup and reloads the save.

Before deleting:

1. Save or discard other pending grid changes.
2. Select only entries you have positively identified.
3. Read the storage and status columns.
4. Never delete an unknown entry only because its name is missing.

Light red rows are mission or friendship-quest items and require extra caution. Normal recognised quest and friendship rewards already owned by the save are not marked red.

## 18. Full JSON Editor

Open **Tools > Full Editor** for advanced inspection.

The Full Editor includes:

- formatted JSON display;
- syntax highlighting;
- line and position information;
- Format JSON;
- Validate;
- Search;
- Copy;
- Undo and Redo;
- Export Decrypted JSON;
- Import Decrypted JSON;
- Save.

The same supported Evolving actions are also available from the Full Editor's Tools menu.

### Export Decrypted JSON

Creates a readable JSON copy for comparison or careful external inspection. Exporting does not change the active save.

### Import Decrypted JSON

Loads a complete modified JSON file into the Full Editor.

The imported file must:

- be valid JSON;
- contain the expected save root;
- include the required GameInfo, Player, and World structures.

Import creates safety backups and keeps the imported data in the editor until Save is selected.

### Saving in the Full Editor

The editor parses and validates the JSON before writing it. Invalid JSON is blocked and reports useful line or position information.

After saving, the Full Editor keeps the visible document formatted and readable. The actual profile file may still be written compactly, which is normal.

Manual JSON editing is the highest-risk part of the editor. Do not change sections you do not understand, and never replace large objects with guessed data.

### Convert String to JSON helper

The separate **Tools > Convert String to JSON** utility converts simple two-column text such as an item ID followed by a name into a formatted JSON dictionary.

This helper is mainly useful to advanced users preparing or checking item lists. It does not edit the loaded save automatically. Review and copy its output only when you understand where that data belongs.

## 19. Saving and validating a save

### Normal category edits

Use **Tools > Save** after changing rows in the main category tabs.

The editor writes the supported categories as one batch and reloads the save. Check for a successful status and confirm that the player name and level still appear correctly.

### Immediate actions

Some repair, delete, memory, house-floor, and bulk actions write immediately after confirmation. Their dialog explains what will happen.

### Validation

For manual JSON work:

1. Select **Validate**.
2. Fix every reported error.
3. Confirm the expected save root still exists.
4. Save only when validation succeeds.

For normal grid work, the editor reload after Save provides an additional practical check that the profile can still be parsed. The final check must still happen inside the game.

### In-game test

After editing, check:

- the game starts;
- the save loads;
- the player name and progress are correct;
- backpack, furniture, wardrobe, map, and Collection open;
- quests and memories appear normally;
- changed items are in the expected place;
- Evolving tools remain selectable and usable;
- no new loading error appears.

## 20. Common warnings and errors

### No save loaded

Load profile.json before using category, repair, or save actions.

### Please select profile.json

The selected file has the wrong name or is not the active save profile.

### Error loading Save file

Possible causes include a damaged file, wrong file, unsupported structure, inaccessible path, or incomplete decryption. Restore a backup before trying more edits.

### Invalid JSON

The Full Editor or imported file contains a syntax error. Use the reported line and position, fix the structure, and validate again.

### Protected or excluded item skipped

The item is intentionally blocked from that operation. Do not work around the protection by forcing it through JSON unless the exact save requirement has been verified.

### Item already exists

Adding another copy could create a duplicate. Find the existing entry first and edit its amount or status if appropriate.

### Profile limit reached

The activation already has the maximum number of save profiles. Contact support for review rather than registering another email on the same computer.

### Profile registered elsewhere

The save identity is connected to another activation. Support must review the legitimate owner and existing profile link.

### Editor version no longer authorized

Old releases can be disabled when they are unsafe or incompatible. Download the newest official build and do not mix its files with the old folder.

### Update message appears

**Editor Data Updated** is informational. The newest supported item data and corrections are ready.

## 21. Safety rules

Never:

- edit while the game is running;
- work without an untouched backup;
- share profile.json publicly;
- mix files from different editor releases;
- add random IDs found online without verifying their purpose;
- delete unknown or light-red entries only to make a list look clean;
- use manual JSON to bypass a protected-item warning;
- add only the final variant of an Evolving tool;
- reduce inventory size while items remain in disappearing slots;
- run several repair tools without testing between them;
- use extreme currency or item amounts without understanding the result.

Known unsafe or blocked examples:

- **Pixel Dust** must not be added or edited.
- **Pooh's Thoughtful Spot, ID 40005832**, cannot be newly added.
- Mission and friendship-quest objects should not be added or deleted casually.
- Protected tools, skins, mounts, gliders, memories, and other excluded entries should remain protected.

Prefer individual additions over Add All when only one or two items are needed.

## Final reminder

The safest workflow is simple:

**Backup → load the correct save → make one clear change → save → test in game.**

The editor provides powerful tools, but careful use is more valuable than changing everything at once.
