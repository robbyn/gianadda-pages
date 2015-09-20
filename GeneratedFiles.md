---
layout: default
title: Generated files
permalink: /GeneratedFiles.html
---
# Generated files

Gianadda creates a number of subdirectories when it generates a gallery:

* `_site` is the actual generated website. You can browse it locally or upload it to a web server,
* `_theme` contains a copy of the theme files. You usually don't want to change its content, unless
you want to customise the theme on a per-gallery basis. When you change the theme of the gallery with the `--change-theme` option, the old theme is saved as `_theme.backup`.
* `_catalog` contains a database with all the information collected from the pictures and folders in the gallery structure (note to hackers: it's an [H2](http://www.h2database.com/) database).
