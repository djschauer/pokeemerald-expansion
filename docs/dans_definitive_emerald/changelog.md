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

Reasoning: The design goal for Dan's Definitive Emerald is to maintain the original feel of the Base Emerald game with just some Quality of Life features to smooth out the Gameplay experience.

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

Reasoning: As part of stage 1 I wanted to maintain Emerald's original typings and learn sets, and added in a couple of useful QoL things like HM Delete and Dynamic Typing showing up. I also maintained the confirmation prompt on move deletion since I like it, but I may revisit this setting later.

## 2026-07-04

### Updated battle.h File

Changes:
- Updated Most Damage and Calculation settings back to Gen 3, except in cases where I felt a more modern interpretation made sense
- Updated Experience settings to allow for Catch XP, evenly split XP on switches, everything else was set to Gen 3
- Badge boost was set to Gen 3 (Emerald behavior) and the settings are default
- All type and turn settings were set to Gen 3
- Moves will retain their Gen 3 Typing and Stats, but their tags will have their modern updates
- All Accuracy settings are at their Gen 3 levels
- All stat changes except for Growth and Focus Energy (I may revisit Charge and Rapid Spin)
- Most other Move and ability settings were set to Gen 3 except in cases where it wouldn't likely be relevant or made sense
- Moves with turn limits were maintained a their defaults
- Most Battle Items were set to Gen 3 settings
- Most if not all specialty Balls were given their highest catch rate setting
- Move Description in Battle is enabled, visible with L
- Ability weather is set to Gen 3, the remaining Weather related settings are Gen Latest
- Most Interface settings are at True, Run from Trainer battle is False
- Crit Capture is on, based on Regional dex (I beleive that is how that setting works)
- Catch bonuses mostly increased, excpet for Gen 8/9 Low Level bonus
- Enabled all new animation settings (will revisit after testing)
- Enemies throw pokemon into battles enabled
- Show Types and Effectiveness set to Never (May revisit in the future)
- Move Rearrangement in battle allowed

Reasoning: The intention with these changes was to maintain balance as much as possible, while allowing for updates that make sense or particularly with Catch rate, interface, and things like Last Ball and Move Description.

### Successful Build

## 2026-07-06

### Reverts and Updated Items and Fishing

Changes:
- Reverted Pokemon Sprites and Animations to Original Emerald (May revisit this later, some new Sprites I liked others I didn't)
- Fixed the Mist weather setting, accidentally left that on.
- Reverted the KO and Pokeball Animations (again, some I liked and some I did not, may revist later)
- Added Infinite TMs
- Fixed Nature Power to use Gen 3 options
- Set fishing mechanics to be Gen 3
- Made Escape Rope a Key Item
- Set EXP Share to be Gen 6 style, toggleable Key Item that gives XP to the whole party
- Vitamins can go over 100 EV Cap
- Held Items like Charcoal that boost types were set to their more modern 1.2 boost (may revisit if this throws off balance too much)
- Most other Item setting retained their Gen 3 Mechanics

Reasoning: The reversions were based off of playtesting the latest build and the game just not looking like Emerald in Battle at times, specifically Nosepass and Lombre threw me off. Although some of the sprites I really did like, but this first iteration I want the OG look. Infinite TMs is just a must for me, as well as the modern exp share saving on grinding. The rest were easy choices for maintaining Gen 3 feel.

### Successfuly Build

## 2026-07-07

### Primarily overworld.h

Changes:
- Running Indoors was left Enabled (big QoL)
- Whiteout cutscene where pokemon are healed enabled
- Move Tutors let you pick from PC and Party not just Lead pokemon
- Left all the Berry stuff alone
- Chose to forego Follower Pokemon for now, will update on a separate branch so that I don't bork anything (did enable weather forms for Castform as followers)
- Set all out of Battle ability effects to Gen 3 (may revisit later, some of these seem cool)
- Pokedex plus left disabled
- Updated Pokerus to show on Eggs, which is Emerald behavior
- Added IVs/EVs to the summary screen
- IVs are displayed as letters, which I think is aesthetically pleasing (may revisit later and expose the actual numbers)
- Moves can be relearned via the summary screen rather than requiring a trip back to Fallarbor (May revisit later)
- Allowed Pokemon to relearn moves from Previous evolutions


investigate : Better HMs in the field, Berry eat animation, infinite bag, Trade evos