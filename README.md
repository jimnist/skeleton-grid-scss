skeleton-grid-scss - IN PROGRESS
==================

i need a fixed grid system for a project built using [spree commerce](http://spreecommerce.com/) which currently uses [Skeleton](http://www.getskeleton.com/), but in a pretty wacked way (imho).

i need to use a grid for a layout that can work with existing template code (which specifies grid containers and columns in the html) and for pages that i create and templates that i override, i want to keep that out of the markup and use SCSS includes.

i also am including a slightly simpler layout, with variables for breakpoints, which can easily be overridden.

this is ONLY the skeleton grid, not the other parts of the framework.

this is a mashup of these differnt projects:
* [Skeleton](https://github.com/dhg/Skeleton)
* [skeleton-sass](https://github.com/atomicpages/skeleton-sass)
* [Skeleton-SASS](https://github.com/lazerwalker/Skeleton-SASS)
* with a little bit of inspiration from [Profound Grid](http://www.profoundgrid.com/)

##files




##usage

##development

there are LOTS of different ways to compile the [SCSS](http://sass-lang.com/) into CSS.

i normally use [Compass](http://compass-style.org/), but since this is not dependent on any of the compass features, during development, i compile with the __sass__ utility by running:
```
$ sass --watch scss/your-app.scss:stylesheets/your-app.css
```

i use [Livereload](http://livereload.com/) (on a mac) to monitor changes on the disk and refresh the browser.


