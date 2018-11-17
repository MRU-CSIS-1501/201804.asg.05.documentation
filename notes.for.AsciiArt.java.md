# Notes for AsciiArt.java

## Background

We need to create a class to capture all the details about ASCII art. This is a very important class and deserves some attention!

When you begin this assignment, we won't have covered files yet (but will shortly thereafter). To work around this, this class defaults to creating art objects that don't come from a file - they come from a constant that is defined in the class. Hello Kitty!

## What's provided to you already

- completed constructors `public AsciiArt()` and `public AsciiArt(String filePath)`
  - you will need to complete the `init()` method for these constructors to work properly
  - for the constructor that takes in a file path, you will need to do a bit of extra work - see the docs for more details
- constant `DEFAULT_ART`
  - this String is the art used to create an object when the no-arg constructor is called

## What you need to complete

There are a number of sections in the code marked TODO - you need to complete each one. (Please remove the TODO when you have completed the method.)

If you need to create any helper methods, they should be declared **private** and **non-static**.

## What you can assume

You can assume you won't be asked to make an AsciiArt object from an empty file.