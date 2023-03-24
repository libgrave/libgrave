
# libgrave

libgrave is hopefully going to be a DOS game programming library targeting
16-bit real mode and optimized to have reasonable performance even on
8088 @ 4.77MHz PCs like the original IBM Model 5150 and Compaq Portable.

It is inspired by the late 1990s versions of Allegro game programming
library, thus the name. Grave is a very slow and solemn (24–40  bpm) tempo
in music, where Allegro is fast and bright (100–156 bpm).

Most of the libary is probably going to be written in MASM 5.1 comatible
assembly, with high level game loop being in C. I'm not sure what C
compiler to chose, contenders at the moment are:

- Turbo C++ 3.0
- Microsoft C/C++ 7.0
- Watcom 11.0c / OpenWatcom 1.9

One thing I strongly consider for libgrave is EMS memory support. There is
very little software / games that will run on 8088 CPU and can take
advantage of EMS memory. This needs to change.

I'd like to get support for the following graphics hardware:

- Hercules
- CGA
- Plantronics ColorPlus
- EGA
- VGA
- VESA 1.2 SVGA

I'd also like to get support for the following sound hardware:

- Adlib
- CMS / GameBlaster
- Sound Blaster up to 2.0
- Covox and SoundSource
- OPL2 or OPL3 on LPT
