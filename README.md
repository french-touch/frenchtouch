# FRENCHTOUCH.dev

## TODO

## BUILD

1. build locally

> python wrapper.py -l
> cd www_folder
> python -m http.server

2. build locally and push to github pages

> python wrapper.py -l
> cp www_folder to ghpage folder
> git commit | push

Note to build locally in a way compatible with CNAME `RELATIVE_URLS` has to be set to `True` in `pelicanconf.py` or via -e RELATIVE_URLS=`True`

## DEPLOYMENT

### Git Hub Pages

> Already at works [frenchtouch.dev](https://frenchtouch.dev)

## DOCUMENTATION

### Templates

`template/base.html` defines the base template for the website
`template/index.html` super's the content with the list of articles (and adds a header with categories)

### Javascripts added

`super-search.js`: uses the sitemap.xml generated to provide easy search for site's posts
`Mathjax v3.2.2`: used for rendering maths nicely

### Globals

List of pelicanconf.py globals used

AUTHOR
FEED_ALL_ATOM set to `"feed.xml"` needs to be aligned with values in `super-search.js` for the .js to find content and allow local search
PATH
STATIC_PATHS
SITENAME
SITE_LOGO
SOCIAL: modified from default Pelican to be 3-uple for displaying under Sitename (includes font awesome name)
OUTPUT_PATH
PLUGINS
    sitemap
    more_categories
    MARKUP (requires `Markdown` package to be installed or fails silently)

## CREDITS 

> See Credits
