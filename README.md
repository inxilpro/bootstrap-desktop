# Twitter's Bootstrap (3+) — without media queries

Bootstrap 3 went mobile-first, which means that browsers that don't support media queries got much more complicated to support.  The Bootstrap documentation recommends using [Respond.js](https://github.com/scottjehl/Respond), but this often introduces performance issues and other bugs.

This is a "desktop-only" version of Bootstrap, which has all media queries stripped from it, and serves the "medium" version of Bootstrap (simulating a 1024px wide display).

## Usage

Use conditional comments to load the desktop version of Bootstrap for MSIE 8 and below:

    <!--[if gt IE 8]><!-->
    <link href="path/to/bootstrap.css" rel="stylesheet" />
    <!--<![endif]-->
    <!--[if lt IE 9]>
    <link href="path/to/bootstrap-desktop.css" rel="stylesheet" />
    <![endif]-->

## Underlying Technology

Whenever a new version of Bootstrap is released, I run the released CSS through a build process that regenerates it using [grunt-stripmq](https://github.com/jtangelder/grunt-stripmq).  For more information, [see my blog post explaining this project](http://cmorrell.com/?p=8).