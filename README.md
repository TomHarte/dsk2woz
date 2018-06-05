# dsk2woz
A command-line tool to convert Apple II DSK images to WOZ format.

Usage:

    dsk2woz input.dsk output.woz

Reads the contents of the DOS 3.3 disk input.dsk and outputs the WOZ-format file output.woz.

## Building
There are no dependencies beyond the C standard library. So e.g.

    cc dsk2woz.c -o dsk2woz
