# eSpeak Text-to-Speech for Espeakedit

This is just temporary [eSpeak NG fork](https://github.com/espeak-ng/espeak-ng/) for espeakedit compilation!

espeakedit is a GUI frontend which allows one to prepare and compile phoneme
data for the [eSpeak NG](https://github.com/espeak-ng/espeak-ng/) speech synthesizer.

Ensure that versions of dictionary data produced by espeakedit and
consumed by espeak/espeak-ng are compatible.

Note, that there is ongoing effort to develop modern version of [EspeakNG Java Editor](https://github.com/valdisvi/espeak-ng-jeditor)
which is not ready jet, but contributors are welcome.

## Build Dependencies

Solve dependencies for [eSpeakNG](https://github.com/espeak-ng/espeak-ng/#dependencies)

On Ubuntu 16.04 LTS "Xenial Xerus", it requires to install following additional packages

sudo apt install libportaudio2 sox libwxgtk3.0-dev portaudio19-dev

This binary is can compiled to use `V19` of the PortAudio library.  If you have
`V18` you will need to recompile espeakedit, after copying `portaudio18.h` to
replace the original `portaudio.h` file in the src directory.

## Building

The espeak and espeakedit programs, along with the espeak voices, can
be built via the standard autotools commands:

	$ ./autogen.sh
	$ ./configure --prefix=/usr
	$ make -B

## Documentation

Look at:

 * http://espeak.sourceforge.net/editor.html
 * http://espeak.sourceforge.net/editor_if.html
 

## Data

To run espeakedit you ned symbolic link to `espeak-data` folder.
E.g. `espeak-data -> code/espeak-ng/espeak-data/`

Directory `phsource` contains the master phonemes file `phonemes`, additional
phoneme files for various languages, and all the sound files needed to compile
the phoneme data into `espeak-data/phondata`, `phontab`, `phonindex`.

## Links

* http://espeak.sourceforge.net/
* http://www.wxwidgets.org/
* http://www.praat.org/



