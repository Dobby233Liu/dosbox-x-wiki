<img src="images/Demoscene:Jump-by-Public-NMI-(1992).gif" width="640" height="400" style="image-rendering: -moz-crisp-edges; image-rendering: crisp-edges; -ms-interpolation-mode: nearest-neighbor; -webkit-optimize-contrast;"><br>
[[1992|Guide:MS‐DOS:demoscene:1992]] demoscene entry.

# Demo description

(todo)

# Recommended DOSBox-X configuration

    [dosbox]
    memsize=1
    machine=vgaonly
    
    [cpu]
    core=normal
    cputype=386
    cycles=5000
    
    [sblaster]
    sbtype=sbpro2
    sbbase=220
    irq=5
    dma=1
    goldplay=true
    goldplay stereo=true
    # the following are needed to work around bugs (DOSBox-X? Or the demo?) related to PIC masking.
    # they are HACKS to be used until the demo is further examined.
    pic unmask irq=true
    force dsp auto-init=true
    
    # alternatively, if you want to avoid the hacks and run it without problems, use the LPT DAC playback mode (and set cycles=7000)
    [speaker]
    disney=true

To run the demo, type JUMP.BAT

# Bugs

## Sound Blaster IRQ problems

Sound Blaster playback is unreliable due to problems with managing the PIC interrupt mask for the Sound Blaster IRQ. It is not known whether DOSBox-X or the demo is at fault.

Test results so far:

|Hardware|Sound card|Result|
|--------|----------|------|
|Toshiba Satellite Pro 465CDX|Yamaha OPL3-SA2 (Sound Blaster compatible)|"Unlimited shadebob" music plays fine. Music stops after 1-2 seconds in other parts. Same as DOSBox|

## VGA blanking and the dot landscape

The dot landscape does not show up on screen if the cycle count is greater than about 7000. It also fails to appear on-screen on real 486 & Pentium hardware.

# More information

[More information (Pouet)](http://www.pouet.net/prod.php?which=4210)
