---
layout: default
title: Theme templates
permalink: /Themes/ThemeTemplates.html
---
# Theme templates

Some files in a theme are simply copied in the destination folder, while others are used as templates to generate the destination file. Normally, the `.html`, `.css`, and `.js` files are used as templates.

The template engine used is [Velocity](http://velocity.apache.org/). You can read the Velocity User Guide [here](http://velocity.apache.org/engine/releases/velocity-1.7/user-guide.html), and the language reference [here](http://velocity.apache.org/engine/releases/velocity-1.7/vtl-reference-guide.html). Some useful tools are included in Gianadda:

* the [EscapeTool ($esc)](http://velocity.apache.org/tools/releases/2.0/javadoc/org/apache/velocity/tools/generic/EscapeTool.html),
* the [DateTool ($date)](http://velocity.apache.org/tools/releases/2.0/javadoc/org/apache/velocity/tools/generic/DateTool.html),
* the [ComparisonDateTool (also $date)](http://velocity.apache.org/tools/releases/2.0/javadoc/org/apache/velocity/tools/generic/ComparisonDateTool.html),
* the [MathTool ($math)](http://velocity.apache.org/tools/releases/2.0/javadoc/org/apache/velocity/tools/generic/MathTool.html)

## Objects specific to Gianadda

The following Gianadda objects are accessible from within a template:

* `$base`: a relative path to the root of the website. Very handy to build URLs to site-level files such as
CSS or JavaScript files.
* [$conf](/Themes/ConfStructure.html): an object giving access to the settings,
* [$folder](/Themes/FolderStructure.html): the current folder (for a site-level template, this the root folder),
* [$pic](/Themes/PictureStructure.html): the picture being processed (only available to the preview template)

To see examples of templates, you can have a look a the [source files for the default theme](https://github.com/robbyn/gianadda/tree/master/res/themes/default), most notably [folder/index.html](https://github.com/robbyn/gianadda/blob/master/res/themes/default/folder/index.html).
