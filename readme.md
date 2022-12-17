Create a *.desktop* file for a wine executable.

# Install

Requirements are:

- *wrestool* command from *icoutils* package
- *convert* from *imagemagick* package
- *natsort* python module

Then you can invoke *make install* to install this script.

    $ sudo apt install icoutils imagemagick python3-natsort
    $ sudo make install

# Usage

    $ install-wine-desktop path-to-executable.exe
    
# Description

We extract the icon from the executable using *wrestool* command.
Then we convert the icon to *.png* format with *convert* tool and
copy it to *~/.local/share/icons* directory.
Next we create *.desktop* file in *~/.local/share/applications* directory.
