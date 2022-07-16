towave - a program to extract the channels from a chiptune file
(C) 2011 Victoria Mitchell (QuietMisdreavus, formerly icesoldier)
http://icesoldier.me/towave.html

*** about ***

Running towave on a chiptune file will generate a number of WAV files that
correspond to the number of channels available on that emulator. For example,
running towave on a GBS file will generate four files (two squares, one wave
and one noise). The files will be named like such:

	1-Square 1.wav
	2-Square 2.wav
	3-Wave.wav
	4-Noise.wav
	
	(again assuming a GBS file is given)
	
*** use ***
	
Towave must be run from a command prompt. Call it like this:

	towave filename
	
where filename is of one of the types mentioned below. It will then ask which
track of the file to play, followed by how many seconds to record. It is worth
noting that towave records all tracks, even those with no sound data.

(Something interesting I discovered while writing this is that in Windows 7,
you can drag a chiptune file onto the EXE file, and it will run properly. This
way, you don't have to muck around in Command Prompt if you don't want to.)

*** filetypes ***

towave uses the Game Music Emu library, which supports the following filetypes:

AY			(for ZX Spectrum/Amstrad CPC music)
GBS			(for GB, GBC music)
GYM			(for Sega Genesis/Mega Drive music)
NSF/NSFE	(for NES music - see below for further notes)
SAP			(for Atari systems using the POKEY sound chip)
SPC			(for SNES music)
VGM/VGZ		(for Sega Master System/Mark III, Sega Genesis/Mega Drive,
				and BBC Micro music)

A note about NES files: The version of GME I use supports the VRC6, VRC7,
Namco 106, MMC5, FME-7, and Famicom Disk System expansion chips. I'm not sure if
that's all of them, but it's worth noting.

*** contact ***

If you have any questions, comments, bug reports, etc, you can contact me:

The quickest is on Twitter: http://twitter.com/QuietMisdreavus
Otherwise, you can email me at victoria@quietmisdreavus.net

With either method, please mention that you ware talking about towave in your
message.

Enjoy the chiptune goodness!
