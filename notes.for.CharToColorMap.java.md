# Notes for CharToColorMap.java

## Background

If you want to have a piece of ASCII art colored something than white when it's converted, you will need to make a hex color map file with the proper format in the correct location. See the File Notes section [here](./directory.structure.and.file.notes.md) for further details.

`AsciiToPngConverter` objects need a `CharToColorMap` object to tell them how to color the characters that are being converted.

## What's provided to you already

- constant `DEFAULT_COLOR`
  - this is the hex color code for white
  - don't change this - automated tests will fail if you do!

## What you need to complete

There are just three methods (and two of them are constructors!) that you need to do in here - they are marked TODO. (Please remove the TODO when you have completed the method.)

If you need to create any helper methods, they should be declared **private** and **non-static**.