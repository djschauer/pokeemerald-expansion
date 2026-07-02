# Changelog for Dan's Definitive Emerald

## 2026-06-29

### Updated Species Configuration

Changes:
- Restrict all pokemon to Gen 3 only
- Disabled Regional Forms
- Disabled Megas
- Disabled Gigantamax
- Disabled Teras
- Disabled Fusions
- Disabled Cross-gen Evos
- Added Changelog, Design, and feature docs

Reasoning:
The design goal for Dan's Definitive Emerald is to maintain the original feel of the Base Emerald game with just some Quality of Life features to smooth out the Gameplay experience.

## 2026-07-01

### Updated Pokemon.h File

Changes:
- Set types and abilities to be Gen 3
- Set Level Up Learnsets to be Gen 3
- Shedinja Pokeball setting to Gen 3 (does not require pokeball)
- Set no Shinies without Pokeballs to True
- Set Show Dynamic Typing to True, this means things like Hidden Power will show their typing
- Set delete move confirmation to True, meaning it will ask for the additional confirmation
- Set able to delete HMs to True, the plan is to handle HMs cleaner, but this is still a good setting