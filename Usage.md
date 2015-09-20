---
layout: default
title: Usage
permalink: /Usage.html
---
# Usage

```sh
gianadda [-?|-h|--help] [-v|--verbose] [-q|--quiet] [--debug]
    [-s|--sync] [-f|--force-html]
    [(-c|--create) <theme-name>] [(-t|--change-theme) <theme-name>]
    [--tolerance <tolerance>] [--google-browser-key <key>]
    [--google-server-key <key>]
    <gallery-directory>
```

## Options:

<dl>
    <dt>-?|-h|--help</dt>
    <dd>
    Display this help text.
    </dd>
    <dt>-c|--create &lt;theme-name&gt;</dt>
    <dd>
        Create a new gallery using the given theme, in the given directory.
        When used, -s and -f are implied.
    </dd>
    <dt>-t|--change-theme &lt;theme-name&gt;</dt>
    <dd>
        Change the theme of the gallery in the given directory.
        When used, -s and -f are implied.
    </dd>
    <dt>--google-browser-key &lt;key&gt;</dt>
    <dd>
        Set the Google Maps API browser key to be used by the
        static maps service<sup>1</sup>.
    </dd>
    <dt>--google-server-key &lt;key&gt;</dt>
    <dd>
        Set the Google Maps API server key to be used by the elevation
        service<sup>2</sup>.
    </dd>
    <dt>-s|--sync</dt>
    <dd>
        <p>Synchronize the given gallery to reflect changes in the content of the
        gallery directory:</p>
        <ul>
          <li>create new folder when new directories are found</li>
          <li>create new pictures when new image files are found, and generate
                thumbnails and preview files.</li>
          <li>update picture info in the catalog when image files are changed,
                and regenerate thumbnails and preview files.</li>
        </ul>
        <p>NOTE: Unless the --delete is used, he folders and pictures that no longer
                exist in the directory structure are kept in the catalog.</p>
    </dd>
    <dt>-d|--delete</dt>
    <dd>
        Also delete pictures and folders that no longer exist in the directore
        structure.
    </dd>
    <dt>-f|--force-html</dt>
    <dd>
        Force the generation of the html (and css, js, ...) files of the web
        site, whether there was a change or not. When used, -s is implied.
    </dd>
    <dt>--simplify</dt>
    <dd>
        Simplify tracks using a Douglas-Peucker algorithm.
    </dd>
    <dt>--tolerance &lt;tolerance&gt;</dt>
    <dd>
        Specify the tolerance in meters for the Douglas-Peucker algorithm. When
        used, --simplify is implied.
    </dd>
    <dt>-e|--elevation-service</dt>
    <dd>
        Use the Google Maps elevation web service to get the elevation of track
        points.
    </dd>
    <dt>-E|--force-elevation-service</dt>
    <dd>
        Forces the use of the elevation service even when the track points
        already have elevations.
    </dd>
    <dt>-v|--verbose</dt>
    <dd>
        Display information messages. Without this flag, only warnings and
        errors are displayed.
    </dd>
    <dt>-q|--quiet</dt>
    <dd>
        Don't display warning messages (only error messages)
    </dd>
    <dt>--debug</dt>
    <dd>
        Display ALL messages, including debug messages. There can be quiet a lot.
    </dd>
</dl>

# Footnotes

<sup>1</sup> [Google Static Maps API](https://developers.google.com/maps/documentation/static-maps/)

<sup>2</sup> [The Google Maps Elevation API](https://developers.google.com/maps/documentation/elevation/intro)
