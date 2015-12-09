# Steganography ![image](./app/src/main/res/mipmap-xhdpi/ic_launcher.png)

* Hide arbitary data into an image
* 
* 

## General info

Hide arbitary data inside the least significant bits (LSB) of data in an image.

Uses 3 color channels and lsb allowing (3*width*height)/8 bytes of storage


### Example
For a 200x200 pixel bitmap there are 40k pixels, each with 3 channels (rgb) so by hiding stuff in the least significant bit of each channel of each pixel we are able to hide (40k * 3) bits of data or 15kb of data. This might seem like a lot but a raw bitmap of this size is about 1mb of data.


TODO: Library
* Attempts to zip data if it doesn't fit
* AES encrypt (including header), by default so (gen pass) so header is hidden
* Allow using 2*lsb
* Optionally allow usage of the alpha channel

TODO: Example app
* Structure
* Select photo activity
* Select file / message to hide
* Nice errors

## Usage


## Building

It's a standard gradle project.

## 