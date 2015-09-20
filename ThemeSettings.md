---
layout: default
title: Theme settings
permalink: /ThemeSettings.html
---
# Theme settings

A theme may optionally contain a settings.properties files that contains a list of properties that apply to the whole site.

Some of theses properties are used by Gianadda itself, while some others are only used in the theme's [templates](/ThemeTemplates.html).

The following properties are used by Gianadda:

* `preview-size`: size of the preview (large) images. default: `800,600`
* `thumb-size`: size of the thumbnails. default: `150,100`
* `pic-name-pattern`: regexp to filter picture image names. default: `^[^.].*[.](jpg|jpeg)$`
* `dir-name-pattern`: regexp to filter folder names. default: `^[^._].*$`
* `template-name-pattern`: regexp to filter [template](/ThemeTemplates.html) names. default: `^[^.].*[.](html|css|txt|xml|rss)$`
* `preview-template`: name of the preview [template](/ThemeTemplates.html). default: `preview.html`
