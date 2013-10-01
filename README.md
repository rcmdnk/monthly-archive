monthly-archive
===============

Sidebar part of Monthly Archive for Octopress.

# Installation

1. Copy `plugins/monthly_archive.rb` and `plugins/monthly_generator.rb`
   to your `plugins` directory.

1. Copy `sass/plugins/_monthly_archive.scss` to your `sass/plugins/` directory,
   and add a line:

    `@import "monthly_archive"`

   to `sass/plugins/_plugins.scss`.

1. Copy `sass/plugins/_monthly_archive.scss` to your `sass/plugins/` directory,

1. Copy `source/javascripts/monthly_archive.js` to your
   `source/javascripts/` directory,
   and add a line:

    `<script src="{{root_url}}/javascripts/monthly_archive.js"></script>`

   to `source/_includes/custom/head.html`.

1. Copy `source/_layouts/monthly_index.html`
   to your `source/_layouts/` directory.

1. Copy `source/_includes/custom/asides/monthly_archive.html`
   to your `source/_includes/custom/asides/` directory.

Done!

# Usage
Add `custom/asides/monthly_archive.html` to `default_asdies` in `_config.yml`.

# Options

## Sidebar part representation
Sidebar part representation can be changed by options
for `monthly_archive` tag in `source/_layouts/monthly_index.html`.

Use `option:value` for each option:

|Option|Possible Values|Default|Description|
|:-----|:-------------:|:-----:|:----------|
|counter|true/false|true|Show number of posts.|
|first_open|true/false|false|Open the latest year list at first.|
|month_format|Jan/JAN/January/JANUARY/01/1|JAN|Month representation format.|

The default is same as:

    {% monthly_archive counter:true first_open:false month_format:JAN %}

## Index pages title
A title of the index page can be changed in `_config.yml`.

The title is formatted like:

    "monthly_title_prefix""month(monthly_format)" "year"

Possible options are:

* monthly_title_prefix (Default: `Archive: `)
* monthly_format (Possible values are same as above sidebar part. Default: `JAN:`)


# Example
Check `Monthly Arhives` in sidebar of the blog: http://rcmdnk.github.io/.


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/rcmdnk/monthly-archive/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

