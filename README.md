# Desktop-only version of Twitter's Bootstrap

This is a desktop-only version of Twitter's bootstrap (with all media queries stripped).  Useful for serving MSIE 8 and lower without using Respond.js.

## Usage

Use conditional comments to load the desktop version of Bootstrap for MSIE 8 and below:

    <!--[if gt IE 8]><!-->
    <link href="path/to/bootstrap.css" rel="stylesheet" />
    <!--<![endif]-->
    <!--[if lt IE 9]>
    <link href="path/to/bootstrap-desktop.css" rel="stylesheet" />
    <![endif]-->

[See blog post explaining this project](http://cmorrell.com/?p=8)