<img src="images/Demoscene:Panic-by-Future-Crew-(1992).gif" width="640" height="400"><br>
[[1992|Guide:MS‐DOS:demoscene:1992]] demoscene entry.

# Demo description

(todo)

# Recommended DOSBox-X configuration

    [cpu]
    core=normal
    cputype=pentium
    cycles=15000
    
    [dos]
    xms=true
    ems=true
    
    [sblaster]
    sbtype=sbpro2
    sbbase=220
    irq=5
    dma=1

The demo requires expanded memory (ems=true) for Sound Blaster playback.

# Bugs

Some of the demo's raster effects (especially the "scrollers suck" part) become slightly glitchy if run with core=dynamic. The shadebob part runs too fast, causing the rotating dot cube to finish too early.
The plasma raster effect will occasionally glitch if Sound Blaster playback is active.

If Youtube captures like [this](http://www.youtube.com/watch?v=MQDRLOPem48) are any indication, the demo has similar problems on real hardware.

# More information

[More information (Pouet)](http://www.pouet.net/prod.php?which=479)
