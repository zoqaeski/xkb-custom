# XKB Configuration #

These files are used by XKB to generate my custom keyboard mappings.

It's an experimental work-in-progress that almost certainly has bugs because the XKB documentation is so arcane.

## Usage (or how I use this) ##

Drop the files into `$XDG_CONFIG_HOME/xkb/`, and execute something like the following line in a terminal:

    xkbcomp -I$XDG_CONFIG_HOME/xkb/ $XDG_CONFIG_HOME/xkb/keymap/custom.xkb ${DISPLAY%%.*}

The changes take place immediately; you can use `xev` to verify.
