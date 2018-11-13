# Directory structure & file notes

## Directory structure

This assignment has four directories of particular importance: **ascii-art-files**, **color-map-files**, **generated-hexcolor-files**, and **generated-png-files**.

Each of these directories has their own purpose:

- **ascii-art-files** holds the ascii art files you start with as well as any you have created. s well as any associated color map files.
  - each ascii art file should have a **.txt** file extension
- **color-map-files** holds the charcter to color map files you start with as well as any you have created.
  - each color map file should have the same name as its associated ascii art file (_without_ the extension) and have a **.map** extension
- **generated-hexcolor-files** holds any hex color files the user has created for ascii art files.
  - each file in this directory will have the name of its associated ascii art file (_without_ the extension) and have a **.hex** extension
- **generated-png-files** holds any PNG files the user has created for ascii art files.
  - each file in this directory will have the name of its associated ascii art file (_without_ the extension) and have a **.png** extension

Here is what you start with:

<pre>
├── ascii-art-files
│   ├── bat.txt
│   ├── block.txt
│   ├── cake.txt
│   ├── dog.txt
│   ├── jagged-block.txt
│   └── java.txt
├── color-map-files
│   ├── bat.map
│   ├── block.map
│   ├── cake.map
│   └── dog.map
├── generated-hexcolor-files
│   ├── bat.hex
│   ├── block.hex
│   ├── cake.hex
│   ├── dog.hex
│   └── java.hex
├── generated-png-files
│   ├── bat.png
│   ├── block.png
│   ├── cake.png
│   ├── dog.png
│   └── java.png
</pre>

## File notes

### ASCII art files

If you want to make new ASCII art files, you can just create an appropriately named file in Emacs (remember the file must end in **.txt**). I would suggest **not** using spaces in your file names.

If you want to grab something off the internet, you can just paste what you find into an Emacs window.

### Color map files

If you want to color ASCII art files a certain way, you'll need to create an appropriately-name color map file using Emacs.

Each line in the file has the following format:

`[character][space][hex color]`

For example, if you look in the **bat.map** file, you'll see this:

<pre>
" #000099
/ #000099
= #000099
X #000099
\ #000099
^ #000099
_ #000099
i #000099
x #000099
| #000099
  #888888
</pre>

What this is telling you is this: each character in the left-most column except for the space (yes, there's a space on that last line!) is going to be colored with hex color `#000099` ![#000099](https://placehold.it/15/000099/000000?text=+). Each space will be colored with hex color `#888888` ![#888888](https://placehold.it/15/888888/000000?text=+).

### PNG files

These are image files created by turning each character into a single colored pixel. The color is determined by the associated color map file. If no color map file is provided, then the default color for every character/pixel is white!

You can view the images using FileZilla. See the FileZilla info for more detail.

### Hex color files

These are just like the PNG files - except that instead of pixels, we have hex color codes. These files will be used in the automated marking process.
