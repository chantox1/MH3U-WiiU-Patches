# MH3U-WiiU-Patches
**(mostly) Obsolete, see [MH3U WiiU Patcher](https://github.com/chantox1/MH3U-WiiU-Patches).**

For EU game version.

# Usage / Installation

Use only one patch.

For Cemu emulator:

Locate your game's update data (referred to as v32 or 1.02). This should be in an extracted format, with 'code', 'content' and 'meta' folders.

Within 'code', locate 'MH3G_Cafe_EU.rpx'. Using [xdelta UI](https://www.romhacking.net/utilities/598/), select the desired patch and MH3G_Cafe_EU.rpx, give the output file a temporary name, and place it in the code folder. Rename MH3G_Cafe_EU.rpx to MH3G_Cafe_EU.rpx.bkp (any name works, this is just a backup). Then, rename the output file you gave a temporary name to to MH3G_Cafe_EU.rpx.

Finally, in the Cemu emulator, install (say yes if asked to reinstall) the update data under File -> Install game title, update or DLC.

If patching fails, please verify MH3G_Cafe_EU.rpx matches the following MD5 hash: 382289663eb3bf8a73884260690449d8

# Patches

DefTo1: Several mh games add a fixed amount of defense to the player regardless of armor. In MH3G, this is a flat +1 defense, as is the standard. In MH3U, however, this is a +50, likely intended to make the western localization more accessible by making it easier. This patch reduces that 50 defense down to 1, for parity with MH3G.

RawDebloat: Weapons in several mh games (MH3U included) feature 'bloat values', which are multipliers to a player's attack, dependent on weapon type, intended to showcase how slower weapons such as GS or Hammer deal more damage per hit. As these values are visual-only, obscuring the real attack values without impacting gameplay, they tend to be disliked in the mh community. This patch forces all bloat values to 1x, so true attack is shown on all weapons.

# Special Thanks
IncognitoMan for pointing out how bloat values are stored
