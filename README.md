# Neav UI

## Changes and additions

#### oUF_Neav:

- Different short value formatting (e.g. 1.1m instead of 1M 100K).
- Added Blizzards holy power, eclipse and soulshard bars, they fit the UI very nicely.
- Added boss frames

#### Raid frames:

- Now using the built-in heal prediction from oUF (kind of like healcomm).
- Healing indicators for all classes (I hope), as well as soulstone, focus magic and dark intent.
- Healing indicators now have a "cooldown spiral" for duration.
- Mouse-over indicator (darkening the color when hovering over a frame).
- Disabled smooth updates for healing classes (can be enabled via `oUF_NeavConfig.lua`).
- Mana bars (enabled in `oUF_NeavConfig.lua`)

#### nMainbar:

- Option to have a vertical petbar (see `nMainbar_Config.lua`).

#### Misc:

- Healthbar on tooltips now have a textual representation on it as well.
- Added a copy chat function to nChat, use it by right-clicking on the chat tab. Also added a URL copy function.
- nRunes has been removed and replaced by nPower, which is essentially the same thing except with support for energy, focus and rage as well. The energy module also shows combo points in a similar fashion as nRunes showed runes.
- nTooltip: the target of the mouseover unit has now a raidtarget support
- nTooltip has now a reaction coloring for the border and healthbar and itemquality border support!

## Known issues

- ??? The quest blob on the map is still a cause for taint, not really sure what's causing it and if it really needs fixing.
- !Colorz cause an ui-block-error (not lua error!), because we change the value of a global table, ignore this or delete `PowerBarColor['MANA'] = {r = 0/255, g = 0.55, b = 1}` in the `!Colorz.lua` file.

## Next Steps

- test nPlates in raid/instance situations and optimize his code
- `nPlates` find better coloring or a other threat indicator
- skin mdoule for external addons like omen, recount etc.
- unhappy with the raidframe situation
- make the oUF_Neav layout more usefull with tags for class specific buffs
- create arena frames
- nCore module for open all mails (and ignore mails with COD)
- make nPower compact, add config file and put it on wowi

## Ideas

- create lightweight nameplates in neav ui style 
- oUF_Neav - raid frames, get rid of the unit_aura event and use a OnUpdate event instead for better cpu usage?
- remove omen from the ui and create a file/addon which "skin" omen wihout modify the original data (for better updates)

## Installation

## Bugs?

## Credits
- ballagarba for updated this UI.
- Neav for creating this UI.

## Screenshots
