# Notes for AsciiToPngConverter.java

## Background

Since converting an `AsciiArt` object to a PNG file is a non-trivial process, we want to make a class that will help us do the conversions.

`AsciiToPngConverter` objects need three other objects to help them do their job:
- the `AsciiArt` object that's being converted
- a `CharToColorMap` object to tell them how to color the characters that are being converted
- a `Picture` object that is the PNG version of the ASCII art

## What's provided to you already

Nothing - you've got to build this sucker from scratch!

## What you need to complete

There are just three methods, including 1 constructor, that you need to do in here - they are marked TODO. (Please remove the TODO when you have completed the method.)

If you need to create any helper methods, they should be declared **private** and **non-static**.