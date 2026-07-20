# Dreamlight Editor

A portable Windows save editor for Disney Dreamlight Valley, built to make careful changes easier to understand, review, and undo.

Version 0.9.7 adds new editing tools, clearer item handling, automatic editor-data updates, and email sign-in to help keep the editor free and reduce commercial misuse.

📘 **Need detailed instructions?** Open the [complete DDV Wizard Editor User Guide](DDV_WIZARD_EDITOR_USER_GUIDE.md). It explains every category, backup workflow, bulk action, repair tool, warning, and common error.

## ✨ Features

- Load supported Disney Dreamlight Valley `profile.json` save files.
- Browse and edit save content in clear category tabs.
- Search items and filter visible content by expansion.
- Add or remove individual items, including wallpaper, flooring, meals, memories, and other supported content.
- Keep multi-selected rows selected when opening the right-click menu.
- Show items already present in the save even when they are unknown, unavailable, or blocked from being added again.
- Inspect player inventories with **All Save Items (including unknown) - Beta!**
- Use focused fixes for duplicate gliders and Collection progress.
- Manage player-house floors and return furniture from removed floors to the inventory.
- Complete supported Evolving tool and wing progression correctly.
- Open the Full Editor for advanced JSON inspection and careful manual changes.
- Export or import decrypted JSON.
- Receive protected Dict updates automatically without downloading the complete editor again.
- Create backups before important or immediate save operations.

## 🛡️ Safety First

The editor includes several safeguards, but every save edit still deserves care:

- Important file operations create a backup before changing the profile.
- JSON is checked before imported or manually edited data is accepted.
- Invalid JSON is stopped with a useful error instead of being written blindly.
- Existing item data is preserved where the editor supports it.
- Mission and friendship-quest items are highlighted in light red when they need extra caution.
- Normal quest and friendship rewards already owned by the save are not marked as dangerous.
- Known unsafe additions are blocked. Pixel Dust cannot be edited as a currency, and Pooh's Thoughtful Spot ID `40005832` cannot be newly added.
- Items that already exist in a save can still be displayed so an incorrect entry can be found and removed.

Always keep your own untouched copy of `profile.json` before testing an edited save in game.

## 🧾 JSON Export / Import

The Full Editor is intended for advanced inspection and manual work:

- **Export Decrypted JSON** creates a readable copy of the loaded save.
- **Import Decrypted JSON** loads a modified JSON file back into the editor.
- **Format JSON** keeps the document readable.
- **Validate** checks the JSON structure before you continue.
- Search, copy, undo, redo, syntax highlighting, and line information help you review changes.
- Saving inside the Full Editor keeps the JSON formatted instead of collapsing it into one very long line.

Only import a complete, valid save structure. If you are unsure about a manual JSON change, restore the backup and start again.

## 🖥️ Editor / Interface

The main editor provides organized views for supported save content such as player inventory, pets, clothes, houses, furniture, makeup, skins, wallpaper and flooring, meals, memories, and other available categories.

Useful tools in version 0.9.7 include:

- **Expansion filter** — show All Content, Base Game, Eternity Isle, Storybook Vale, Wishblossom Ranch, or Honeyglow Woods across the editor. This changes only the visible list and does not delete anything.
- **Show Missing Dict Items** — display supported items that are not currently in the loaded save, so you can add only what you want.
- **All Save Items (including unknown) - Beta!** — inspect unknown, blocked, or misplaced inventory entries and remove entries you have positively identified as incorrect.
- **Evolving** — add the supported tool or Elegant Firework Wings variants together with their required Level 2 and Level 3 progress.
- **Fix Duplicate Gliders** — remove duplicate glider data and return wing gliders to the correct inventory.
- **Repair Collection From Owned Items (Beta)** — reconnect Collection entries for items the save genuinely owns without adding new inventory items.
- **Manage House Floors** — clear the first floor or remove selected higher floors while returning placed furniture to the Furniture inventory.
- **Memories tools** — manage supported memories while protecting story and quest memories with additional warnings.
- **Automatic Dict updates** — install new item lists and corrections after startup. The editor shows a short confirmation when an update has been applied.

Beta tools are clearly marked because they can touch a wider part of the save. Read their confirmation message and use them only for the problem they describe.

## 📦 Download

1. Open the newest version on the repository's **Releases** page.
2. Download the ZIP file for the latest official build.
3. Extract the complete ZIP into a new folder.
4. Start **Dreamlight Editor - Public.exe** from that folder.

The editor is portable and does not need to be installed. Do not run it from inside the ZIP, remove required files, or combine files from different versions.

If Windows reports a missing runtime, install the free **Microsoft .NET 8 Desktop Runtime (x64)**.

## 🚀 How to Use

1. Close Disney Dreamlight Valley.
2. Start the editor and enter your email address.
3. Enter the six-digit sign-in code sent directly to your inbox.
4. Open **Tools > Load Save** and select the correct `profile.json`.
5. Check the displayed player name and level before editing.
6. Make the changes you need in the category tabs or Tools menu.
7. Use **Tools > Save** for normal editor changes.
8. Start the game and check the result carefully.

Sign-in is normally remembered, so you should not need a new code every time the editor starts. One activation is intended for one Windows PC and can be linked to up to three different save profiles.

Email sign-in was introduced because a small number of people used the free editor to make money from other players. The goal is to limit that misuse while keeping normal access simple for the community.

## ⚠️ Important Notes

- Keep an untouched backup of your original save.
- Never edit a save while the game is running.
- Test a few changes at a time.
- Some repair and management tools save immediately after you confirm them.
- Do not delete mission, quest, or unknown entries unless you understand why they are in the save.
- Do not mix the executable or Dict files from different editor versions.
- Do not post your `profile.json` publicly.
- The editor uses only the information needed for activation, abuse prevention, and reliable access. Normal save contents are not uploaded as part of the sign-in process.
- Save editing can affect progression or game data when used carelessly.

## 🧪 Recommended Testing

After saving, open the game and check that:

- the game starts and the edited profile loads;
- the player name and progress still look correct;
- inventory, furniture, wardrobe, map, and Collection pages open normally;
- quests and memories still appear as expected;
- edited items or values appear in the intended place;
- upgraded tools remain selectable and usable;
- no new warning or loading error appears.

When reporting a problem, include the editor version shown at the top, the category or tool used, what you expected, what happened instead, and a screenshot if possible.

## 🧰 Troubleshooting

- Restore the newest backup if the game no longer loads the edited profile.
- Undo the most recent change and test again with a smaller edit.
- Confirm that the ZIP was completely extracted and that all included files remain together.
- Make sure you are using the latest official release.
- Check the spam folder if the sign-in email does not appear immediately.
- Use **Validate** in the Full Editor after any manual JSON change.
- If imported JSON is rejected, confirm that it is valid JSON and still contains the complete expected save structure.
- If an automatic data update is applied, restart the editor before checking the updated item list.
- Share save files only through a private support channel.

## 💙 Disclaimer

Dreamlight Editor is an unofficial fan-made tool. It is not affiliated with, endorsed by, or supported by Disney, Gameloft, or Disney Dreamlight Valley.

Use it at your own risk and respect the game, its players, and the work of the people who maintain this free community tool.
