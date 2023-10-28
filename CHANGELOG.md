# 2.5.0
* Updating Manifest to begin testing for V11 compatibility.

# 2.4.2
* Fix zip file reference that was causing wrong version of the module to be downloaded.  Special thanks to @thatlonelybugbear for helping to find the issue.

# 2.4.1
* Minor update to version v10 compatibility range

# 2.4.0
* Updated dice-tooltip to be compatible with FoundryVTT 10.  This version breaks compatibility wiht FoundryVTT 9.  Use 2.3.1 if you still want to use this module with FoundryVTT 9.   

# 2.3.1
* Added guard against undefined "item" object, which apparently could happen with MidiQOL and modules that deal with automation.

# 2.3.0
**This module now requires use of DND5e system 0.95 or later.**
* Fixed handling of scaling cantrips which caused an error to display in the console and no tooltip to appear.  This was due to a change in the DND5e 0.95 system module.
* Fixed stylesheet conflict with chat log's dice tooltip's.  Renamed all of mine to use "dtt2" prefix instead of "dice-tooltip"

# 2.2.2
* Fixed stylesheet conflict with SmallTime module

# 2.2.1
* Minor fix to versioning

# 2.2.0
* Now render both normal & versatile damage in one tooltip
* Verified compatibility with FoundryVTT 9

Bug Fixes:
* Fixed ability save rendering.  It had been displaying "d20 - NaN"
* Updated module.json to include Portuguese locale listing.  Not sure if using that locale was broken before, but this should help
* Fixed corner case for constant folding where you could end up with a "+ 0" in the expression. It's now properly removed
* Remove damage types injected in the middle of formulas using "[type]" notation.  We add a label at the end of the roll, so it doesn't need to be in the middle.

# 2.1.1
* Minor fixes
* Updated README to convey recent improvements
* Added pictures to the README

# 2.1.0
* Simplified dice expression display using redundant operator removal and constant folding
* Implemented ability to show tooltips on Tidy5e favorites
* (internal) fixed spelling errors within the source code

# 2.0.1

* Removed "2" from all titling to keep original "dice-tooltip" package name.
* Renamed module: dice-tooltip2 -> dice-tooltip as part of that

# 2.0.0

* Forked from https://github.com/SteffanPoulsen/dice-tooltip to https://github.com/trev33b/dice-tooltip2
* Renamed module: dice-tooltip -> dice-tooltip2
* Fixed compatibility with Foundry 0.8 & Tidy5eSheets
* Improved the tooltip presentation (tightened padding, inverted coloring to match other tooltips, add transparency)
* Fixed dice formula presentation to not show extra +'s
* Changed Short Rest tooltip to show remaining hit dice that can be used
* Removed unnecessary special handling for Tidy5e (Player & NPC) and Sky's Alt 5e sheets
* Lots of code cleanup (warnings & patterns) and wrapped with WebStorm project
* Added localization support and provided translations for English

# 1.0.8

* Added support for "Tidy5e Sheet" NPCs (https://github.com/sdenec/tidy5e-sheet)

# 1.0.7

* Added support for "Tidy5e Sheet" (https://github.com/sdenec/tidy5e-sheet)
* Fixed an issue where supported sheet modules would have doubled events (performance improvement)

# 1.0.6

* Redid the hit-dice tooltip code, now works for multi-classing as well.

# 1.0.5

* Fixed an issue when having multiple character/npc sheets open at the same time.

# 1.0.4

* Fixed a breaking bug that caused the tooltip to malfunction on various overlays
* The code is now less rigid in regard to how actor sheets handle their id structuring.

# 1.0.3

* Now works with "PopOut!"

# 1.0.2

* Now works with "Sky's Alternate 5th Edition Dungeons & Dragons Sheet"

# 1.0.1

* Added compatibility for FoundryVTT 0.6.0
* Added compatibility for D&D5E System 0.91

# 1.0.0

* Released to FoundryVTT
