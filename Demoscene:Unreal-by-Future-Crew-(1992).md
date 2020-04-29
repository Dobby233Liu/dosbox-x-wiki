<img src="images/Demoscene:Unreal-by-Future-Crew-(1992).gif" width="640" height="400" style="image-rendering: -moz-crisp-edges; image-rendering: crisp-edges; -ms-interpolation-mode: nearest-neighbor; -webkit-optimize-contrast;"><br>
[[1992|Guide:MS‐DOS:demoscene:1992]] demoscene entry.

# Demo description

(todo)

Two versions of the demo were released. Version 1.0 (unreal.zip), and version 1.1 (unreal11.zip). Version 1.1 has Gravis Ultrasound support but removes the funny back-and-forth between two scrollers in the second part.

# Recommended DOSBox-X configuration

    [dosbox]
    machine=vgaonly
    memsize=2
    
    [cpu]
    cycles=25000
    core=normal
    cputype=386
    
    [sblaster]
    sbtype=sbpro2
    
    [gus]
    gus=true

Version 1.1 of the demo has GUS support. For v1.0, select "Sound Blaster Pro".

# Bugs

Version 1.0 Sound Blaster playback will stop after part 3 (World Vector).

The vectorballs part (both versions) will flicker if the cycles count is between 8000 and 22000. Not sure if this is a DOSBox-X bug or a bug in the demo.

# Future enhancements for DOSBox-X

Version 1.0 apparently supports the [Sound Master II](http://www.vgmpf.com/Wiki/index.php?title=Sound_Master_II). Version 1.1 replaces that selection with Gravis Ultrasound support.

# More information

[More information (Pouet)](http://www.pouet.net/prod.php?which=1274)
