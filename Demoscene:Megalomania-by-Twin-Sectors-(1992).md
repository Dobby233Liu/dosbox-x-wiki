<img src="images/Demoscene:Megalomania-by-Twin-Sectors-(1992).gif" width="640" height="400"><br>
[[1992|Guide:MS‐DOS:demoscene:1992]] demoscene entry.

# Demo description

A demo that plays music while using hardware color palette animation to scroll text. After that, there are some 3D dot landscapes and objects to show off.

# Recommended DOSBox-X configuration

    [dosbox]
    memsize=2
    machine=svga_et4000
    
    [cpu]
    cputype=386
    core=normal
    cycles=12000
    
    [sblaster]
    sbtype=sbpro2
    sbbase=220
    
    [speaker]
    initial frequency=0

The demo starts with a high resolution 640x480 256-color logo. This SVGA logo requires an ET4000 to display properly.

The demo will turn on and leave on the PC speaker for some reason. Set initial frequency to work around that issue.

Sound Blaster support does not require IRQ or DMA resources. It uses IRQ 0 and direct DAC commands to play music. The demo can also use parallel port DACs, a Covox on 0x2CF (?), and the PC speaker as audio output. PC speaker output is not recommended because the demo amplifies the music too much to the point of clipping audibly.

# More information

[More information (Pouet)](http://www.pouet.net/prod.php?which=58777)
