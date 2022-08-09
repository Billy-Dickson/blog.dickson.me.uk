---
layout: single
title:  "Exiftool - Remove exif data from photographs"
date:   2022-03-20 13:37:08 +0000
categories: computing, linux, commandline
publish: false
---

## Howto remove exif data from photos

Here's a handy linux command line tool that removes exif data from photographs, This one I use to remove the exif data from photos before I publish them to my website.

## Install the appication

~~~bash
sudo apt install exiftool
~~~

### Show the metadata

~~~bash
exiftool photo.jpg
~~~

### Show metedata for all *.jpg files. Note: The extension is case sensitive

~~~bash
exiftool -ext jpg
~~~

### Same as above, but include sub directories

~~~bash
exiftool -r -ext jpg .
~~~

### Remove all metadata

~~~bash
exiftool -all= -overwrite_original photo.jpg
~~~

### Remove all metadata of all *.jpg files in the current directory

~~~bash
exiftool -all= -overwrite_original -ext jpg
~~~

### Does the same as above, but includes subdirectories

~~~bash
exiftool -all= -r -overwrite_original -ext jpg .
~~~

### Remove all GPS metadata of *.jpg files in the current directory

~~~bash
exiftool -gps:all= *.jpg
~~~

## References

[Linux Nightly](https://linuxnightly.com/how-to-remove-exif-data-via-linux-command-line/)
