# ErgoDox EZ Svorak A5 

This layout is supposed to be an implementation of the [Svorak A5
layout](http://aoeu.info/s/dvorak/svorak).
Unfortunately, the Ergodox EZ lacks one column for the right hand, why the
three buttons furthest to the right, on the right half, are missing.
I have tried to move them around and have yet to find a perfect position for them.

## Use the Swedish Software Keyboard

The keyboard assumes that the operating system interprets your keyboard as
Swedish. If you get weird issues (like, most letters work, but not all special
characters) please make sure your operating system uses a Swedish keyboard
layout.


## Note

The keyboard assumes that the operating system interprets your keyboard as
Swedish. If you get weird issues (like, most letters work, but not all special
characters) please make sure your operating system uses a Swedish keyboard
layout.


## Flashing

### Ubuntu

In order to compile and flash your Ergodox EZ, invoke the following at the root
of the repository.

`make ergodox_ez:dvorak_svorak_a5:teensy`

<<<<<<< HEAD
### WSL2

1. Download QMK: 
 
    `python3 -m pip install --user qmk`

2. Setup QMK in WSL2

    `qmk setup`

3. Install [QMK Toolbox](https://github.com/qmk/qmk_toolbox)

    [Downloads](https://github.com/qmk/qmk_toolbox/releases)

4. Compile the HEX in WSL2

    `make ergodox_ez:dvorak_svorak_a5`

5. Flash the keyboard in Windows using QMK Toolbox
=======
I haven't gotten the above to work on Windows. Instead I use
[Msys2](https://www.msys2.org/) to compile the .hex-file (`make ergodox_ez:dvorak_svorak_a5`)
and [Teensy Loader](https://www.pjrc.com/teensy/loader_win10.html) to flash the
board.

>>>>>>> Fix issue with special characters

## Changelog

* 2021-05-04
  * Rebase on upstream (after three years)...

* 2018-08-10
  * Make special characters work in Windows
  * Add QWERTY layer

* 2018-08-09
  * Initial release
* 2018-08-10
  * Make special characters work in Windows
  * Add QWERTY layer
* 2020-10-21
  * Add umlaut (¨)
  * Add F11 to first layer
  * Remove some duplicates from the symbol layer

## Author
Erik Thorsell
erikthorsell @ github and twitter
