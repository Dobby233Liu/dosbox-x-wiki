<img src="images/Demoscene:Inside-by-CNCD-(1996).gif" width="640" height="400"><br>
[[1996|Guide:MS‐DOS:demoscene:1996]] demoscene entry.

# Demo description

(todo)

# Recommended DOSBox-X configuration

    [dosbox]
    memsize=16
    machine=svga_s3
    
    [cpu]
    cycles=max    # set to 250000 if you want to capture instead
    core=dynamic
    cputype=pentium
    
    [sblaster]
    sbtype=sb16
    
    [gus]
    gus=true

GUS emulation should be enabled so the demo can automatically choose it for best music audio quality. You should run SETUP.EXE to configure the demo for Gravis Ultrasound GF1 hardware mixing. The high cycles count is needed for the 3D objects and effects used in the demo. If you only want to watch the demo instead, you should consider cycles=max instead. Note that the README.TXT also strongly recommends "a fast Pentium".

The demo may sit at a black screen for up to 30 seconds before running at startup. Be patient before killing the DOS session and restarting.

# More information

[More information (Pouet)](http://www.pouet.net/prod.php?which=74)
