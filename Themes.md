---
layout: default
title: Theme
permalink: /Themes/
---
# Themes

To generate a gallery web site, Gianadda need a theme. A very basic theme (named default) is provided with the generator, other themes may be built in the future, but they will be in a project of their own.

## Theme structure

A theme is either a directory, or a zip file with the extension `.ggt`, `.jar`, or `.zip`.

It contains the following elements:

<dl>
<dt>settings.properties (optional)</dt>
<dd>
    <p>A list of property definitions, to be used in the whole site.</p>
</dd>
<dt>preview.html (optional)</dt>
<dd>
    <p>A template to be used to generate an HTML page for each picture of the site.</p>
</dd>
<dt>folder</dt>
<dd>
    <p>A directory containing all the files and templates needed to generate the HTML files in
    each folder of the gallery.</p>
    <p></p>
</dd>
<dt>site</dt>
<dd>
    A directory containing all the files and templates needed to generate the HTML files in
    each folder of the gallery. You would normally put all the theme's images, CSS files,
    and JavaScript files in this directory, or a subdirectory.
</dd>
</dl>

It's not a bad idea to also include a README file.

* [Settings](/ThemeSettings/)
* [Templates](/ThemeTemplates/)
