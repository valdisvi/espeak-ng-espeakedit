# eSpeak Text-to-Speech for Espeakedit

This is just temporary [eSpeak NG fork](https://github.com/espeak-ng/espeak-ng/) for espeakedit compilation!

## Build Dependencies

On Ubuntu 16.04 LTS "Xenial Xerus", it requires the following packages
to run:
 * `libwxgtk3.0`
 * `libportaudio2`
 * `sox`
 * `libwxgtk3.0-dev`
 * `libportaudio-dev`

## Building

The espeak and espeakedit programs, along with the espeak voices, can
be built via the standard autotools commands:

	$ ./autogen.sh
	$ ./configure --prefix=/usr
	$ make


