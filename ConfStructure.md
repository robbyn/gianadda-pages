---
layout: default
title: The $conf object
permalink: /ConfStructure/
---
# The $conf object

The **$conf** object gives access to all the Gianadda settings. It's a map of strings.

To access a property, you would use the notation `$conf['name']` or `$conf.name` if the name only contains identifier characters.

You can also access properties as integers (`$conf.ints['name']`), booleans (`$conf.bools['name']`), or dimensions (`$conf.dims['name']`). Dimensions are object with a `width` and a `height` property.

For instance, to get the height of thumbnails, you would write: `$conf.dims['thumb-size'].height`.
