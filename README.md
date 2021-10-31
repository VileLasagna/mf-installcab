# November 2021 Notice

Merged patches by Galcian79 which collect the archive files from a different location which is still available
 ~Vile Lasagna

# December 2020 Notice

This may be broken with prefixes created with Proton 5.13, due to permission issues with how they symlink dll files.

# May 2020 Notice

For many games this script is not needed anymore, and may soon not be needed at all.

This is largely thanks to work Guy1524 has done in officially implementing Media Foundation support into Wine. I would reccommend trying games with latest Proton-GE first, and only using this as a backup.

# mf-installcab
Installcab based Media Foundation workaround for Wine

Just set WINEPREFIX and run install-mf-64.sh like this

`WINEPREFIX="/dev/brain/wine prefixes can be anywhere/folder" ./install-mf-64.sh`

Then copy the included mfplat.dll to the same directory as the `.exe` (e.g. re2.exe)

Steam stores Proton Wine prefixes as \<STEAM FOLDER\>/steamapps/compatdata/\<GAME ID\>/pfx

Optionally you can use Proton's Wine instead of your system's Wine. See script for how.

installcab.py is the same as upstream with very small differences (https://github.com/tonix64/python-installcab/blob/master/installcab.py)

### Dependencies
- python
- cabextract
- wine (optional if proton used)
