---
layout: default
title: The `$folder` object
permalink: /FolderStructure.html
---
# The `$folder` object

The `$folder` object gives access to information related to the current folder.

## Folder attributes

* `id`: unique ID number,
* `parent`: parent folder,
* `subfolder`: list of the subfolders,
* `pictures`: list of the [pictures](PictureStructure) contained in the folder,
* `name`: name of the folder (as in the filesystem),
* `title`: title of the folder (default to the name),
* `description`: description text,
* `level`: level in the folder hierarchy (0 for the root folder),
* `path`: path relatively to the root folder,
* `urlPath`: URL-encoded path,

## Folder methods

* `getPicture(name)`: returns the [picture](/PictureStructure.html) with the given name, or `null` if none is found,
* `getFolder(name)`: returns the subfolder with the given name, or `null` if none is found
