# Notes for ArtiiApp.java

## Background

This is the command centre of the assignment - objects from this class will interact with the user, displaying the menu, and reacting to user input until the user wishes to quit.

It might help to think of `ArtiiApp` objects as a manager in a company - they don't do a lot of work themselves, but have a lot of minions that they boss around and tell what to do. (My apologies to any managers out there...but from where I'm sitting....)

With that in mind, `ArtiiApp` objects have the following minions:
- a `Scanner` object to handle keyboard input
- an `AsciiArt` object that represents the ASCII art image currently loaded
- a `CharToColorMap` object that is associated with the current ASCII art image
- an `AsciiToPngConverter` object that can be used to convert the current ASCII art image
- a `FileHelper` object to assist with making sure the right file names are being used (and to help out with a few other file-related things)

## What's provided to you already

- constant `ROOT_DIR`
  - this is the location of the AsciiArtii directory in your home directory
  - you need this to make your `FileHelper` objects

## What you need to complete

You only need to complete the two public methods TODO. One of them is the constructor. (Please remove the TODO when you have completed the method.)

You will also have to create **numerous** helper methods; otherwise, your **run()** method will be insanely hard to understand! These helpers should be declared **private** and **non-static**.

## IMPORTANT NOTE

When you display the unique characters in the current ASCII art, you need to replace the space character in the display (' ') with this character: █ 

Why? I thought it looked better - with just a blank in the display, it wasn't obvious whether that was supposed to be a space...or was a bug! 
