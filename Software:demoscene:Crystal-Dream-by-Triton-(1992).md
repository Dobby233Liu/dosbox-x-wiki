<img src="images/Demoscene:Crystal-Dream-by-Triton-(1992).gif" width="640" height="400"><br>
[[1992|Guide:MS‐DOS:demoscene:1992]] demoscene entry.

# Demo description

A vector object show with raytracing art.

# Recommended DOSBox-X configuration

    [dosbox]
    machine=vgaonly
    memsize=1
    
    [cpu]
    cycles=12000
    
    [sblaster]
    sbtype=sbpro2
    sbbase=220
    dma=1
    goldplay=true
    goldplay stereo=true

# DSP busy cycle technique

Crystal Dream does not concern itself with the IRQ of the Sound Blaster, in fact, it ignores it. Instead, it uses the timer interrupt to watch the DSP's busy cycle while the DMA block is playing. If it sees the busy cycle stop, then it issues another playback command to keep it going. This technique is effective on Sound Blaster and Sound Blaster Pro cards because the DSP's busy bit will cycle periodically while audio is playing or recording.

On clone hardware, where there is no busy cycle, the demo's Sound Blaster routines work regardless because they effectively then [[nag|Hardware:Sound-Blaster:Nagging-the-DSP]] the DSP to restart the block constantly and audio playback runs properly anyway.

However, this demo is not able to play music on Sound Blaster 16 hardware. The reason is that the [[Sound Blaster 16 DSP busy cycle is always running|Hardware:Sound-Blaster:DSP-busy-cycle]], whether or not any audio playback is occuring, so the demo never senses the end of the DSP block and never issues any further commands to keep audio playback going.

Sound Blaster playback is rendered [[goldplay|Libraries:Goldplay]]-style, using a 1 or 2 byte DMA buffer and the timer interrupt.

# More information

[More information (Pouet)](http://www.pouet.net/prod.php?which=463)
