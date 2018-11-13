# Notes for Picture.java

## Background

In order to create PNG images easily, we need a class to do the heavy lifting for us.

Fortunately, Princeton University had some legal-to-use code that did just that - this Picture class.

## What's provided to you already

There are quite a few methods available in here; we only need the following:

- `Picture(int width, int height)`
  - this is the only constructor for this class that we'll be using
- `int height()`
- `int width()`
- `void setRGB(int col, int row, int rgb)`
  - this is used to make a pixel at a given row and col a certain rgb color
- ` void save(String name)`
  - saves the picture to a file with a given name
  - the name must be a valid location!
  - the name must have a **.png** extension!
- ` String toString()`
  - returns a String representation of the picture, with every pixel represented by a hex color code

## What you need to complete

This sucker is DONE. You don't need to add anything here.
