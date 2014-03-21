StretchyTanks is by the great Ancient Gammoner.

This addon is by NathanKell, e-dog, and swamp_ig, featuring models by Tiberion and further textures by Chestburster and Dante80.

This addon to Stretchy Tanks adds a conic tank, two Stretchable SRBs, a new texture system, and some fixes.
*Node size scales when resizing super-stretchy tanks
*stock ST texture stays in aspect when stretching tanks
*will show all resources in tank when you mouseover
*Proper integration with Modular Fuel Tanks or Real Fuels (REQUIRES MFT v4/RF v4 or above!) - when done stretching, go into action editor->tank setup and update each fuel amount the desired amount to get your final amount.
*and a few other misc logic tweaks

Note when using with Real Fuels: Stretchy SRB is ModularEngines enabled, so your thrust will be corrected when not in vacuum. It is also techlevel enabled, although only Isp will change (not casing mass).

The new texture system works off confignodes. There is a file in the StretchyTanks/Parts folder called STTextures.cfg that defines the textures. You can create your own textures, place them in any location, and use ModuleManager to add the appropriate nodes to the STRETCHYTANKTEXTURES node. All documentation on the node syntax is in the STTextures.cfg file.

Note: this SUPERCEDES any prior Stretchy Tanks-related work by either NathanKell or Starwaster.

INSTALL:
DELETE YOUR OLD STRETCHYTANKS FOLDER in the KSP/GameData folder. Then unzip this folder to KSP/GameData
You may also find, in the StretchyTanks/Parts folder, a Template file with the grit layers I use to make the tanks look slightly worn. Feel free to use it and make (and post!) new textures!

License remains CC-BY-SA 3.0 Unported

Changelog
v8.2 =\/=
*Final pre-Procedural Parts release
*Moved RF tanks over to RF mod. Will no longer clutter partlist
*Deprecate non-superstretchy tanks (available to old craft but hidden in part list)
*Support RF v6
*Fix heatProduction for SRBs when using DRE
*Add "utilization" factor: essentially a hack to allow you to copy real rockets. Fat short tanks should have lower utilization; long tall tanks should have higher. Example values: Titan II lower stage: 0.87. Saturn V lower stage: 0.8. Titan II upper stage: 0.7. Atlas D through I: ~0.85. ***NOTE: you MUST rescale the tank slightly after changing utilization or the volume won't update. After that, you can scale it back.***


v8.1 =\/=
*Fixed fuels being re-added at launch for non-MFT/RF users.
*Fixed BlueSides repeating
*Fixed sea level SRB nozzle giving blackscreens (thanks to DYJ and swamp_ig)
*swamp_ig: support tweakables, add structural tanks, refactor code
*updated tank descriptions


v8 == \/ ==
*0.23 compatibility.
*Fixed StretchySRB issue with thrust reverting due to .23 issues.
*Fixed to work with MFT v4 or RF v4.
*Should work properly for non-MFT/RF users again (finally!)

v7 == \/ ==
*Fixed balloon tank to no-surf-attach, lowered crash tolerance
*Added Service Module super-stretchy
*Added new conic tank by e-dog
*Added technode-based radius limits by e-dog
*Added nodeSizeScalar to support Realism Overhaul
*Fixed node issue, where it was not set properly on load (affected procedural fairings and KJR).
*No longer changes shader when KerbPaint present
*Added new nozzles for the Stretchy SRBs by Tiberion

v6 == \/ ==
*Added height and width display
*Changed scaling steps (slightly finer control). Hold LeftShift for 10x speed.
*Removed width and height limits
*Added even-meter tanks (0.5m, 1m, 2m, 3m, 4m)
*Added one new texture by me
*Added three new textures by Chestburster
*Added three new textures by Dante80
*Resized a couple textures, for hopefully no loss in quality.
*Added Balloon-type superstretchy. Needs MFSC v3.3 or above.
*Fixed surface attachment problems (I think)

v5 == \/ ==
*Changed texture handling system. Now all textures are specified in the CFG file.
*Fixed MFS integration again, no ModuleManager patch needed (modules are in the part cfgs)
*added Vacuum-nozzle StretchySRB
*Added five new textures by Chestburster

v4 == \/ ==
*Fixed MFS integration. Requires MFS v3 full or above
*Tech nodes added

v1-v3 were from before this readme; features included:
*node size scales on radial stretch
*textures scale on stretch, keeping aspect ratio intact.
*shows all resources on mouseover
*SRB included with MFS support
*redone MFS support
*3 new textures by NathanKell

============== Original Docs by AncientGammoner: ==============
Gone are the days of having to stack countless smaller fuel tanks only to not get the exact size you really wanted!

Made from a highly advanced material that can stretch to over 100 times its smallest size, with StretchyTanks you can get the exact the amount of fuel and oxidizer you want, every time! Or go wild and stretch it until it can't stretch any more! (warranty void if stretched beyond reasonable limits).

StretchyTanks come in all 5 common tank diameters and can be filled with LiquidFuel/Oxidizer, LiquidFuel, Oxidizer, or MonoPropellent! Now with tons of other neat stuff!


======= Release Notes: =======
Update - v0.2.2 (8-26-13)

-Fixed issues with saving/loading the tank type/texture
-Changed crash tolerance of tanks from 100 to 10
-Breaking Force/Torque now scale with tank size
-Added "Oxidizer" to the list of tank types

Update - v0.2.1 Hotfix (8-21-13)

-Fixed a bug in the loading of LiquidFuel/MonoPropellent tanks

Update - v0.2.0 (8-21-13)

-Fixed it so surface attachments stay on the surface even as the tank stretches
-Fixed some texture issues
Tons of new features added:
-Hovering GUI on mouse-over telling you how much of each Resource is in the tank along with the Total Mass and Dry Mass.
-Ability to switch a tank in the editor to store LiquidFuel or MonoPropellent (in addition to the standard LiquidFuel/Oxidizer).
-Introduction of the SuperStretchyTank that can stretch in width in addition to length.
-Ability to change the texture of the tank on the fly in the editor to an alternative "stock" looking texture.
(read How to Use for further instructions)

Update - v0.1.1 (8-18-13)

-Fixed some bugs
-Added tentative support for Modular Fuel Tanks (unzip the cfg file in place to use)

Release - v0.1.0 (8-16-13)

-Initial Release

======= How to use =======
After installation the fuel tanks will appear under the Propulsion tab. Add them to your vehicle like a normal fuel tank.
If you wish to increase or decrease the size of a tank while building your vehicle: mouse over the tank in question, hold "r" , and move your mouse up or down to stretch the length.
If the tank is a SuperStretchyTank, you can hold "f" and move your mouse side to side to stretch the width. The amount fuel in the tank will update automatically, and is now displayed on a GUI that appears when you hover over the tank.
While mousing over a tank, press "g" to change the fuel type and press "t" to change the texture.

Source included in Plugins folder of download. This is my first plugin for KSP and is by no means a finished work, so if you find a bug don't hesitate to message me or post it here. Thanks!

This work is licensed under a Creative Commons Attribution-ShareAlike 3.0 Unported License.