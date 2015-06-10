monthly-archive
===============

Sidebar part of Monthly Archive for Octopress.

# Installation

1. Copy `plugins/monthly_archive.rb` and `plugins/monthly_generator.rb`
   to your `plugins` directory.

1. Copy `source/_layouts/monthly_index.html`
   to your `source/_layouts/` directory.

1. Copy `source/_includes/custom/asides/monthly_archive.html`
   to your `source/_includes/custom/asides/` directory.

1. Copy `source/javascripts/monthly_archive.js` to your
   `source/javascripts/` directory,
   and add a line:

    `<script src="{{root_url}}/javascripts/monthly_archive.js"></script>`

   to `source/_includes/custom/head.html`.

1. Copy `sass/plugins/_monthly_archive.scss` 
   to your `sass/plugins/` directory.

   If you have old octopress
   (if your `sass/screen.scss` doesn't have `@import "plugins/**/*";`),
   you may need to add

    `@import "monthly_archive"`

   to `sass/plugins/_plugins.scss`.

Done!

# Usage
Add `custom/asides/monthly_archive.html` to `default_asdies` in `_config.yml`.

# Options

## Sidebar view representation

Sidebar view can be set in **_config.yml**.

|Option|Possible Values|Default|Description|
|:-----|:-------------:|:-----:|:----------|
|monthly_archive_count|true/false|true|Show the number of posts.|
|monthly_archive_open|first/latest/all/nil|Define the first view if each year's list is opened or not. first or latest: open only the latest year. all: open all years. nil or any kind of values: close all years.|
|monthly_archive_format|Jan/JAN/January/JANUARY/01/1|JAN|Month view format.|

## Index pages title

A title of the index page can be changed in `_config.yml`.

The title is formatted like:

    "monthly_title_prefix""month(monthly_format)" "year"

Possible options are:

* monthly_title_prefix (Default: `Archive: `)
* monthly_format (Possible values are same as above sidebar part. Default: `JAN:`)


# Example
Check `Monthly Arhives` in sidebar of the blog: http://rcmdnk.github.io/.
