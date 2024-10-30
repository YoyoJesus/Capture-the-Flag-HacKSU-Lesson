# Description

How about some hide and seek? <br>
Download this file here.

# Solution

Download the file and unzip it to start. 

The hints suggest looking into the metadata of the image file within the folder, so a quick google search can get us an online tool to view that information.
I used [exif.tools](https://exif.tools/) specifically for this challenge.

This tool also exists in a cli version on linux machines.

Uploading the image gives all of its metadata, the attribution tag looks especially interesting.
```
cGljb0NURntNRTc0RDQ3QV9ISUREM05fYTZkZjhkYjh9Cg==
```
The '==' tells me that this string may be base64 encrypted.

By putting that text into [dcode](https://www.dcode.fr/base-64-encoding) with Base64 decoding the flag could be found.