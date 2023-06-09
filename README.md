<h1 align="center">
    <a href="https://game-master.net/">UO:Siege Perilous</a><br>
    <img src="https://raw.github.com/ColloidSP/UOSPLinux/main/uo-siege-perilous-icon.png" width="100"><br>
    <a href="https://www.classicuo.eu/">ClassicUO</a> World Map Markers
</h1>

A simple repository to store the map marker points to be used with the World Map in the
[ClassicUO](https://www.classicuo.eu/) client.

![example](https://imgur.com/jvjntAD.gif)

## Installation

- [Download](https://github.com/ColloidSP/UOSP-Map-Markers/archive/master.zip) this repository.
- Extract all the files into `Data\Client` located at the root of the ClassicUO folder.
- Open the World Map or right-click and select `Reload markers`.

If you just want to download the map icons, [click here](https://raw.githubusercontent.com/ColloidSP/UOSP-Map-Markers/master/MapIcons.zip).

## Format

Creating your own marker file is simple. Create an empty file and enter it using this format:

`x,y,mapindex,name of marker,iconname,color,zoom level`

`x` and `y` are the coordinates for the marker.

The `mapindex` defines what map the client must be on for the marker to display. `0` for `map0.mul`, `1` for `map1.mul`, etc.

The `name of marker` is just that, the name you want to see in the map or when you hover over the marker.

The `iconname` must match the name of the image in the `Data\Client\MapIcons` folder. If no icon exists, it will display a simple dot using the color defined. Icons can be created as `.cur, .png, .jpg, .ico` files.

For `color`, the supported values are `red, green, blue, purple, black, yellow, white, none`.

`zoom level` defines when the icon will show/hide when zooming.  `0 = furthest` and `9 = closest` so if you had a marker zoom level set to 1 (for example dungeon entrances), it will show at any zoom level except if you're all the way out (at 0). Default level is 3.

## Helping

If you want to make improvements or help out, submit a Pull Request or message
Colloid on the [UO:Siege Perilous Discord](https://discord.gg/GwRuSV9vAb).

## Acknowledgements

These markers are forked from the [UO:Renaissance map markers](https://github.com/markdwags/uor-markers)
repository kindly provided by [Quick](https://github.com/markdwags/).
