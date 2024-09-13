# drkhrse Arcade Vertical CRT Overlay
CRT overlay for vertical arcade games on TrimUI Smart Pro using [CrossMix-OS](https://github.com/cizia64/CrossMix-OS). I did not get a preconfigured SDCard so I made this set of additions that can be added to CrossMix-OS to add a Vertical Arcade system and did not want to use the Best Collections folder. This supports 4:3 and 16:10 (mainly because I felt like 16:10 was a good compromise between 4:3 and 16:9 for most schmups) aspect ratios with shaders with a crt-geom type of distortion. I chose to base it on the FBNeo emu config files, but you can utilize what I have here to mod it to whatever system you prefer. Tested with the built in scraper and it seems to work ok for me. The overlay itself could be used for other 16:9 systems like the Retroid Pocket 3/4/5 as long as you use the same shaders.

<img src="/screenshots/vertical_16_10_example.png" width="49%">  <img src="/screenshots/vertical_4_3_example.png" width="49%">

## Installation and Setup
These instructions are for a TrimUI Smart Pro with CrossMix-OS installed and working.
1. For the CrossMix-OS formatted SD card, unzip the file and copy over to the SD card. This does not have overwrite/replace any existing files.
2. You may need to enable the emulator for it to show up. Use the **Menu Button > Edit >** Check the **Arcade Vertical** icon in the list.

The default setup is setup for 16:10 video aspect ratio, vertical control remapping, and fake-CRT-Geom.glslp shader. The default icon in this pack is for use with the Burst! them with centered icons and no system labels.

## For 4:3 Display Aspect Ratio
1. **Menu Button > Advance Menu** to goto Retroarch menu.
2. **Quick Menu > On-Screen Overlay > Overlay Preset > vertical_4_3.cfg**
3. **Video > Scaling > Aspect Ratio > 4:3**
4. To save settings go to **Quick Menu > Overrides > Save Content Directory Overrides** to apply to all games in the folder or **Save Game Overrides** to save specifically for that game. I like to keep some games at 4:3 myself, like Ms. Pac-Man.

## Shaders
By default I set the shader to fake-CRT-Geom since that seemed to be fast and didn't cause moire like zfast_crt_geo did at times. You can try some of the other shaders that have similar distortion and see if you prefer them.
- fake-CRT-Geom-potato.glslp
- fake-CRT-Geom.glslp
- zfast_crt_geo.glslp
- zfast_crt_geo_svideo.glslp

If you get confused by any of these setup steps, check out the very detailed [article](https://retrogamecorps.com/2024/09/01/guide-shaders-and-overlays-on-retro-handhelds/) and [video](https://www.youtube.com/watch?v=srlJmZc3Ho4) by Russ at Retro Game Corps details how to use overlays, filters and shaders, much better than I get into here.

## To Do
- Create versions with overlays for shaders that are not distorted to CRT mask.

## Acknowledgements
Big thanks to the [CrossMix-OS](https://github.com/cizia64/CrossMix-OS) devs, Russ at [Retro Game Corps](https://retrogamecorps.com/), and everyone who contribute to the community at the Retro Game Handhelds discord and the [TrimUI subreddit](https://www.reddit.com/r/trimui/) . **Enjoy!*
