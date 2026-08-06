# DDV Wizard Editor 0.9.9

Changes since `0.9.8-hardened-14`.

## Player Inventory and item handling

- Added a searchable Player Inventory catalogue with categories, adjustable amounts, and clear quest-item warnings.
- Added ID-only item entry where supported and corrected Player Inventory field labels to Item ID and Amount.
- Individual right-click additions now unlock only that item's existing Collection entry instead of completing an entire Collection group.
- Added a Scrooge Store display filter alongside the expansion filters.
- Completed the supported Paths and Fences catalogues, including newer paving, Green Gulch, Brick, and Edwardian entries, with selectable amounts.
- Add All for Furniture, Clothing, Wallpaper, and Flooring now skips protected quest and friendship rewards.
- Confirmed broken white 2x2 and invalid fence-length variants are excluded from bulk additions.

## New tools and repairs

- Added Floating Island Cleaner with loose-item and full-cleanup modes. Full cleanup preserves the travel well, returns supported placed objects to the correct inventories, and removes loose resources, chest contents, and nested cleanup data.
- Added Scramblecoin figure unlock and ranking-points editing using verified figure data.
- Added Fix Miscategorized & Invalid Items (Beta).
- Added Remove Broken 2x2 Item Variants for confirmed Furniture, Path, and Fence variants without broadly deleting unknown data.
- Added Fix Clothing, Make-up, Tool, Wing & Glider Quantities. Legitimate Clothing and Make-up duplicate limits are preserved.
- Improved Fix Duplicate Gliders so wing-style gliders remain in Clothing / Back while normal ground gliders remain in the Glider inventory.
- Fixed Elegant Firework Wings: the base item is stored correctly and its Level 2/3 appearances are handled through Evolving progress rather than separate inventory entries.

## Duties, houses, and companion bundles

- Added Choose Long-Term Duties with search, current progress, stage, status, normal/ascending/descending sorting, and selected completion.
- Long-term duty progress can be set to an exact lower or higher value without touching daily duties, claimed rewards, or unrelated progress.
- Added verified names and current milestones for Honeyglow Woods, Pooh Sticks, and other supported permanent duties.
- House deletion now persists correctly.
- Misplaced Aurora Borealis (`60100001`) and Meteor Shower (`60100002`) entries are moved from Houses into Environment.
- Added an optional right-click action for verified companion bundle extras.

## Interface and updates

- Moved Save directly beside Tools so it is no longer easily confused with Load Save.
- Updated new dialogs and warnings to follow the selected Light or Dark theme.
- Moved the automatic updater into the internal program folder; it is launched only after a signed update has been verified.
- Simplified the extracted release folder so the public launcher is clearly separated from protected internal files.

## Important update note

- Users on any 0.9.7 build must manually download the new ZIP once and extract it into a new folder.
- Users on 0.9.8-hardened-14 can receive the signed update through the normal automatic updater.
- Files from different releases must not be mixed.

## Known game display issue

Some saves may show **100% for All Areas** while individual expansions or categories remain below 100%. Multiple conservative repair approaches did not change the combined value reliably while the underlying individual Collection data remained correct. Current evidence suggests the combined percentage is recalculated or displayed by the game itself, likely following a game update. The editor does not intentionally set all areas to 100%, and it avoids a risky broad rewrite while the behaviour continues to be monitored.
