# Create and edit BMP for Greentea OS

Some BMPs in Greentea are particularly sensitive to changing the color depth (number of bits per pixel) and compression type. Such files, for example, are `6.bmp` and `14.bmp` from the `ntoskrnl/inbv/logo`. If the file `14.bmp` changes the compression type or the color depth, then the system will not boot in the debug mode at all.

## What should I do in such cases?

It will be useful to check information about the picture through specialized software, for example, [Full Image Info](http://www.graphicregion.com/imageinfo.zip) (Freeware). Particular attention should be paid to the items `BitsPerSample` and `BMP_Compression`. After that it will be easier to decide what to do with this picture.

* If the picture does not contain compression (BMP_UNCOMPRESSED), then you can edit this picture via Paint and other common graphic editors. The main thing - when saving, specify the same color depth, as in the original picture.
* If the picture is compressed using the RLE (BMP_RLE) algorithm, it can be edited via GIMP. To do this you shall:
  * Open the picture and make corrections to it;
  * Go to "Image" -> "Mode" -> "Indexed" and specify the desired maximum number of colors, equal to 2^(color depth). For example, for a color depth of 4 bits, the maximum number of colors will be 2^4 = 16. After that, the picture will be converted to another color profile.
  * Go to "File" -> "Export As...", specify the type of the file `.bmp`, click "Export";
  * A dialog will appear where you will have to tick off the RLE and check next to "Do not save color space information".
  * Now Greentea may boot with this picture.

Tested with GIMP 2.8.18.
