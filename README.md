# KiCad-Color-Flags
Color flags for use with global labels in KiCad schematics

![Color Flags Used in ESP32 Schematic](https://github.com/rheingoldheavy/KiCad-Color-Flags/blob/main/Examples/esp32_prog_example.PNG)

# Update 31-Oct-2022 (revised)
- "Flags" are meant to be placed inside the global label. "Tags" are colored squares that can be used anywhere.
- KiCad v6 uses a more acute angle for the pointed end of the global label bounding box than v5 did. New polygons have been drawn to reflect this.
- For whatever reason, merely rotating the flag PNG does not make a flag universal between right justified vs. left justified global labels. "R" and "L" polygons have been drawn to work around this.
- ~~The amount of colored space the flag takes up at the front of the global label is different for v5 flags than v6, because v5 does not allow "space" characters. With v6, a larger flag was created for ease of viewing. Adding a leading / trailing space to the text of your global label will accomodate this.~~ In practice, this didn't make any sense. The flags for both v5 and v6 have been adjusted in size so that they do not overlap characters.

## Description
While drafting schematics with complex subsystem interactions, it can be difficult to quickly identify both ends of a global label. These flags can be used to color code those labels within a KiCad Schematic. There are square and pointed flags that can be used either inside or outside of those labels, with 40 mil or 50 mil text size.

![Flag Examples](https://github.com/rheingoldheavy/KiCad-Color-Flags/blob/main/Examples/flag_examples.PNG)

## Use
- Download the KiCad Color Flags zip file from this repository. 
- Unzip into a convenient location.
- Create a global label within your KiCad schematic. Ensure the text size is either 0.040 or 0.050 inches in size.
- Click the "Add Bitmap Image" tool.

  ![Add Bitmap Icons](https://github.com/rheingoldheavy/KiCad-Color-Flags/blob/main/Examples/insert_bmp.png)
  
- Select the color, size and shape of the flag you want to use. If using a pointed flag, indent the label text by a few spaces to expose the flag fully.

Flags named "flag_xx" are square. Flags named "full_flag_xx" are designed to nest inside the pointed end of the global label.

## Flags Included

The proof sheet below is an example of the color and shape of the tags and flags. There are slight variations between those used for KiCad v5 and KiCad v6.

![Proof Sheet](https://github.com/rheingoldheavy/KiCad-Color-Flags/blob/main/Examples/proof_sheet.PNG)
