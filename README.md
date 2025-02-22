# pongo2-addons (for pongo2 v6)

[![Gratipay](http://img.shields.io/badge/gratipay-support%20pongo-brightgreen.svg)](https://gratipay.com/flosch/)

Filter and tag add-ons for [pongo2](https://github.com/flosch/pongo2) (v6)

## How to install and use

Install via `go get -u github.com/astonm/pongo2-addons`. All dependencies will be automatically fetched and installed.

Simply add the following import line **after** importing pongo2:

    _ "github.com/astonm/pongo2-addons"

All additional filters/tags will be registered automatically.

## Addons

### Filters

-  Regulars

   -  **[filesizeformat](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#filesizeformat)** (human-readable filesize; takes bytes as input)
   -  **[slugify](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#slugify)** (creates a slug for a given input)
   -  **truncatesentences** / **truncatesentences_html** (returns the first X sentences [like truncatechars/truncatewords]; please provide X as a parameter)
   -  **random** (returns a random element of the input slice)

-  Markup

   -  **markdown**

-  Humanize
   -  **[intcomma](https://docs.djangoproject.com/en/dev/ref/contrib/humanize/#intcomma)** (put decimal marks into the number)
   -  **[ordinal](https://docs.djangoproject.com/en/dev/ref/contrib/humanize/#ordinal)** (convert integer to its ordinal as string)
   -  **[naturalday](https://docs.djangoproject.com/en/dev/ref/contrib/humanize/#naturalday)** (converts `time.Time`-object into today/yesterday/tomorrow if possible; otherwise it will use `naturaltime`)
   -  **[timesince](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#timesince)/[timeuntil](https://docs.djangoproject.com/en/1.6/ref/templates/builtins/#timeuntil)/[naturaltime](https://docs.djangoproject.com/en/dev/ref/contrib/humanize/#naturaltime)** (human-readable time [duration] indicator)

### Tags

(nothing yet)

## TODO

-  Support i18n/i10n

## Used libraries

I want to thank the authors of these libraries (which are being used in `pongo2-addons`):

-  [github.com/extemporalgenome/slug](https://github.com/extemporalgenome/slug)
-  [github.com/dustin/go-humanize](https://github.com/dustin/go-humanize)
-  [github.com/russross/blackfriday](https://github.com/russross/blackfriday)
