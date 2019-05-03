# mf-installcab
Installcab based Media Foundation workaround for Wine

### Known working games:

- Resident Evil 2
- Darksiders Warmastered Edition

Just set WINEPREFIX and run install-mf-64.sh like this

`WINEPREFIX="/home/gaben/.local/share/Steam/steamapps/compatdata/883710/pfx" ./install-mf-64.sh`

Then copy the included mfplat.dll to the same directory as the `.exe` (e.g. re2.exe)

Resident Evil 2 etc. should then work.

installcab.py is exactly the same as upstream except uncommented lines 129-137 (https://github.com/tonix64/python-installcab/blob/master/installcab.py

The difference between this is a better shell script, and almost no manual intervention needed. It's an extremely simple and short shell script, it's easy to understand.
