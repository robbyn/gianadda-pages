---
layout: default
title: The `$pic` object
permalink: /PictureStructure.html
---
# The `$pic` object

The `$pic` object gives access to the information relative to a picture.

# Picture attributes

* `id`: unique ID number,
* `folder`: [folder](/FolderStructure.html) containing the picture,
* `name`: name of the picture (as in the filesystem),
* `dateTime`: timestamp of the picture. It is either the [EXIF](http://en.wikipedia.org/wiki/Exchangeable_image_file_format) `DateTimeOriginal` attribute (date/time when the photo was taken), if available, the file's timestamp if not,
* `description`: description, as found in the EXIF data,
* `artist`: artist name, as found in the EXIF data,
* `copyright`: copyright message, as found in the EXIF data,
* `width`: image width,
* `height`: image height,
* `path`: path relatively to the root folder,
* `gpsData`: [GPS data](/GpsDataStructure.html) if found in the EXIF information, or null if not,
