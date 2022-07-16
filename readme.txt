towave - a program to extract the channels from a chiptune file
(C) 2011 Victoria Mitchell (QuietMisdreavus, formerly icesoldier)
http://icesoldier.me/towave.html

*** notes about towave ***

towave was a really old project of mine to split out the channels of an emulated
game music file into separate rendered WAV files, so that i could interpret and
understand a track better. (I was writing covers at the time, and for
soundtracks like Streets of Rage 2, it was really helpful.) The program was set
up so that you could drag-and-drop a file onto the EXE, type in the length of
time you wanted to render, and receive a set of WAV files.

I recorded a video demonstrating it: https://www.youtube.com/watch?v=IuU3WlwhI8o

*** notes about the source (2011) ***

Since this was a personal project, I didn't organize the source very much.
However, since I am releasing the source, I figured I'd at least comment it and
tidy it a bit. Also, it's a good way to get this "pre-release" version of GME
I found in the documentation of foo_gep out into the public.

Speaking of GME, the `gme` directory contains the unedited files of gme-0.6-pre.
Oddly enough, this can't be found on Blargg's page nor the semi-official Google
Code page for the library. However, this version contains very important code
allowing support for the VRC7 and FDS expansion chips for the NES. Thus, this
version was chosen for my screwing around in coding.

For the curious, the discussion post where I found the library by itself is here:
http://www.hydrogenaudio.org/forums/index.php?s=&showtopic=30322&view=findpost&p=715125
(While this is a publicly available link, it still has a below-the-table feeling
about the whole business. Maybe someone can clear this out for me?)

*** notes about the source (2022) ***

This source repo contains the "rel3" source dump from icesoldier.me, only edited
to change the human name mentioned in the source, and to add more information to
the readme.

In the time since writing towave, the Game Music Emu library i used was picked
up by Michael Pyne, and updated to build on Linux and macOS. It's available on
Bitbucket here: https://bitbucket.org/mpyne/game-music-emu/ Enterprising
individuals could try to splice it in place of the `gme` source dump i
originally used. PRs welcome!

Given the amount of time since i touched it last, i don't even remember how i
built it! Presumably some invocation like `g++ gme/*.cpp gme/*.c wave_writer.c
towave.cpp` might work, but i can't test that theory, since i don't even run a
Windows machine any more. Since this version of GME directly includes
`windows.h`, it won't build on Mac or Linux. If you can get this running with
CMake or the like, i would love to see a PR!

*** contact ***

Any questions about the source code can be directed to
victoria@quietmisdreavus.net, or to @QuietMisdreavus on Twitter. Please note
though that i haven't touched this project in over a decade, so i may not
remember much about it!

Enjoy the chiptune goodness!
