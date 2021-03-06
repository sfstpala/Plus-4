# Plus-4

This is a pretty simple terminal emulator.

![](http://i.imgur.com/SKv5q.png)

## Installation

To simply install the program on Oneiric, [**download the debian
package**](https://github.com/downloads/sfstpala/Plus-4/src.deb).

If you want to build and install the package, a script is included to
build the debian package:

    cd plus-4/
    ./build
    sudo dpkg -i src.deb

If you're not running Ubuntu, you can just put move `src/opt/plus-4/`
to `/opt/plus-4/` and `src/usr/share/applications/plus-4.desktop` to
`/usr/share/applications/`.

## Keyboard Shortcuts

 - **Ctrl**+**T**: new terminal
 - **Ctrl**+**W**: close terminal
 - **Ctrl**+**Right**: next terminal
 - **Ctrl**+**Left**: previous terminal

 - **F11**: Fullscreen

 - **Ctrl**+**Shift**+**C**: Copy
 - **Ctrl**+**Shift**+**V**: Paste

 - **Ctrl**+**Plus**: increase the font size
 - **Ctrl**+**Minus**: decrease the font size
 - **Ctrl**+**0**: reset the font size

## Configuration

The program's confinguration is at `/opt/plus-4/settings.json`.
It looks like this:

    {
        "font-family": "Ubuntu Mono",
        "font-size": 17,
        "fg": "#7c71da",
        "bg": "#3e32a2",
        "margin": 32,
        "padding": 8,
        "command": ["/usr/bin/env", "bash"],
        "title": "Commodore 64"
    }

## Hackers

If you want to mess with the code, you'll want to check out [VTE's new
documentation](http://developer.gnome.org/vte/unstable/VteTerminal.html).

Notice that it's written (and depends on) Python 3.
