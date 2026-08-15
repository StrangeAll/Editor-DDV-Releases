# DDV Wizard Editor 1.0.0 - Hardened 2

Changes since the previously published `0.9.9-hardened-1`. Internal dashboard changes are intentionally not included.

All bugs reported during testing and since the previous public release were fixed for this build.

The Hardened 2 hotfix restores full-editor updating for already installed 1.0.0 copies while keeping the visible release version at 1.0.0.

## Five save-profile slots

- Following a team decision, every normal user now has five save-profile slots instead of three.
- The editor shows how many slots are in use and how many remain available.
- When the limit is reached, the editor explains that Support must release a slot before another save can be linked.

## Add Items by Source

- Added a selectable `Add Items by Source` window for Premium Items, Twitch Drops, Scrooge Store items, Star Path items, and Event items.
- Multiple sources can be selected and added together in one action.
- A backup is created before the operation.
- Quest rewards, friendship rewards, protected entries, and blocked IDs remain excluded.
- Renamed the narrower bulk option to `Add Edition & Bundle Items` so its purpose is easier to understand.

## Scramblecoin and Touch of Magic

- Added a dedicated Scramblecoin tab for reviewing confirmed figures, inventory amounts, and Collection state.
- Ranking points can be changed and verified figures can be unlocked without replacing unrelated progress.
- Added a dedicated Touch of Magic tab for searching, adding, and removing motifs.
- Existing unknown motifs remain visible with a warning instead of silently becoming addable.

## Safety, comparison, and support

- Added a focused Save Safety Center with useful and actionable findings.
- Added a categorized side-by-side comparison for two saves with friendly file labels.
- Added a preview of unsaved changes before the final save.
- Added a directly visible Undo button and session checkpoints that can restore an earlier editor state.
- Added a private support-package action containing the loaded save, build and Dict versions, diagnostics, safety findings, and session history.

## Collection tools

- Added `Add All Owned Items to Collection (Beta)` for restoring Collection entries for items already owned by the save.
- The action updates owned entries without broadly completing unrelated Collection groups.
- The existing backup-based Collection progress restore remains available.

## Save and Full Editor reliability

- The final `profile.json` is written in the compact encrypted game format instead of remaining as very large plain JSON.
- The compact result is round-trip validated before replacing the original file.
- Saving uses an atomic temporary file to reduce the risk of a partial save.
- The editor accepts both compact game profiles and readable JSON while editing.
- The Full Editor can export readable JSON and import a validated Dreamlight Valley profile before the normal Save action.

## Other reliability improvements

- Improved handling of missing Dict entries and focused inventory repairs.
- The Floating Island Cleaner now handles supported nested values more safely while preserving the selected island's travel well.
- Update checks no longer present a failed-update message when no active full editor update exists.
- The signed updater keeps the previous editor files if installation fails and retries temporarily locked files before giving up.

## Update notes

- The 1.0.0 update is mandatory for supported automatic-updater builds.
- All older editor builds are scheduled to be disabled on **August 19, 2026** because they still contain smaller known issues.
- Users on `0.9.9-hardened-1` can use the signed automatic updater.
- Users still on any 0.9.7 build must download 1.0.0 manually once and extract it into a new folder.
- Files from different editor versions must not be mixed.
