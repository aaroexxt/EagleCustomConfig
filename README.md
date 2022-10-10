# EagleConfig
 My Autodesk EAGLE config scripts w/custom shortcuts etc, for Mac and Windows

Very useful for navigating EAGLE easier, I don't know why they don't include some of these by default :)

## Shortcuts
|Key Combo|When Available|Description|
|---|---|---|
|Alt-C|Layout|Show top layer only|
|Alt-V|Layout|Show top/bottom layers only|
|Alt-B|Layout|Show bottom layer only|
|Alt-X|Layout|Show middle layers (4-layer routing only)|
|Alt-D|Layout|Flip board|
|Alt-R|Layout|Ratsnest (fill polygons with plane)|
|Alt-Shift-R|Layout|Ripup ratsnest (unfill all polygons)|
|Alt-S|Layout|Show airwires (unrouted traces)|
|Alt-Shift-S|Layout|Hide airwires (unrouted traces)|
|Alt-F|Layout|Find component|
|Alt-N|Schematic|Net (run wire)|
|Alt-D|Schematic|Name (name wire)|
|Alt-F|Schematic|Value (assign value to component)|

## Installation

1) Close EAGLE
2) Navigate to your EAGLE installation folder, mine is in Documents/EAGLE_9.x.x
3) Navigate to the "scripts" folder within that directory
4) Rename the existing `eagle.scr` folder to `eagle_original.scr`
5) Copy `eagleWin.scr` or `eagleMac.scr` to the scripts folder, depending on whether you're using Windows or Mac. The only difference is the line extensions.
6) - *Windows*: you need to run the following command inside the scripts directory in order to fix issues with the line endings and the way they are parsed by EAGLE. `TYPE eagleWin.scr | MORE /P > eagle.scr`. See [here](https://stackoverflow.com/a/27844521) for more info.
 - *Mac*: just rename `eagleMac.scr` to `eagle.scr`. The line endings should work out of the box.
8) Reopen EAGLE, you should be all set!
