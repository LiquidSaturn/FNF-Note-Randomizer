# Changelog
All notable changes will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

# [Unreleased]

### Added

- Added the ability for the note randomizer to generate new notes, and turn existing/new notes into hold notes of varying length

### Changed

- The whole codebase was redone from the ground up
- Changed the way some of the save variables work, old saves will be perfectly compatible but some settings changed their location in the save so specific settings may need some reconfiguration but it's not a big deal

### Removed

- OPTIONS.txt was made obsolete by setting descriptions being added to the game, so I saw no reason to keep it

# [2.0.1] - 2025-04-28

### Fixed

- Set the API version in _polymod_meta.json to 0.6.3 so FNF 0.6.3 will load it

# [2.0.0] - 2025-04-06

### Added

- You can now use the options menu to toggle many different settings of the note randomizer

- You can now save (and load) Randomizer Presets! There are also some included by default

- There is now a "Setup SubState" that lets you select whether or not to use the note randomizer alongside various other options when entering PlayState (enabled by default)

- There is now an "Auto Activate" setting that automatically sets the note randomizer to active with the current settings when loading into a song (overwritten by the option chosen on Setup SubState if that is active)

- There are now options to change the frequency of "wave" notes (the third to last note)

- You can now change how long the note queue time is for doubles and triples

- You can now make it so that the randomizer becomes biased for or against notes that get generated more often and notes that aren't generated often

- Made it optional for true random to be allowed to stack notes directly on top of one another, true random cannot stack notes by default

- New debug option which traces a lot of things if you open the game in a cmd window

- The text on the side in PlayState will now say what mode the randomizer is in

- Added an option to reset your save

- Songs you play with the randomizer on no longer save the stats you get on them (at first it looks like it does but upon reloading the rating will disappear)

### Changed

- Improved the ability of the randomizer to recognize patterns and made a more dynamic system to accommodate them

- Full recode to make the project more sustainable, easier to read, and better for future-proofing

- Removed randomizeOnStart because everyone unanimously decided randomizing in real time was just the worse option and it took a lot of unnecessary code space