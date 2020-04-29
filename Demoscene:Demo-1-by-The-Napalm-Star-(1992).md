<img src="images/Demoscene:Demo-1-by-The-Napalm-Star-(1992).gif" width="640" height="400" style="image-rendering: -moz-crisp-edges; image-rendering: crisp-edges; -ms-interpolation-mode: nearest-neighbor; -webkit-optimize-contrast;"><br>
[[1992|Guide:MS‐DOS:demoscene:1992]] demoscene entry.

# Demo description

Basic demo with badly composed music, messages, and 3D rotating objects on a starfield.

# Recommended DOSBox-X configuration

    [dosbox]
    machine=vgaonly
    memsize=1
    
    [cpu]
    cycles=15000
    core=normal
    cputype=386
    
    [dos]
    ems=false
    umb=false
    minimum mcb segment=1400
    
    [sblaster]
    sbtype=sbpro2

You will be prompted to enter Sound Blaster base and IRQ information when starting the demo.

# Low memory issues

Demo will crash after prompting for configuration if the EXE is loaded below segment 0x1400.
Use "minimum mcb segment=1400" param or run LOADFIX twice to resolve the issue.

# More information

[More information (Pouet)](http://www.pouet.net/prod.php?which=4247)
