# dsk2woz
A command-line tool to convert Apple II DSK images to WOZ format.

Usage:

    dsk2woz input.dsk output.woz

Reads the contents of the disk `input.dsk` and outputs the WOZ-format file `output.woz`.

## Building
There are no dependencies beyond the C standard library. So e.g.

    cc dsk2woz.c -o dsk2woz

## DOS 3.3 versus Pro-DOS
Apple II DSK images contain implicitly-ordered sectors; the order depends on whether the image contains a DOS 3.3 image or a Pro-DOS image.

For the purposes of this tool if the file extension of the input disk has a 'p' in it then it is treated as a Pro-DOS image. Otherwise it is treated as a DOS 3.3 image.
