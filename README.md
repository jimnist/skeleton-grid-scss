skeleton-grid-scss
==================

i need a fixed grid system for a project that uses [spree commerce](http://spreecommerce.com/) which currently uses [Skeleton](http://www.getskeleton.com/), but in a little bit of wacked way (imho).

i need to use a grid for a layout that can work with existing template code (which specifies grid containers and columns via classes in the html) and for pages that i create and templates that i override, i want to keep that out of the markup and use SCSS includes.

i also am including variables for breakpoints that are used for calculations. these which can easily be overridden to provide a bigger maximum grid (which i need).

skeleton-grid-scss is based on Skeleton v1.2.

Note that this is ONLY the skeleton grid, and does not include other parts of the framework.

remember that Skeleton is a mobile LAST responsive grid. otherwise, you will be confused.

this is a mashup of these different projects:
* [Skeleton](https://github.com/dhg/Skeleton) - CSS only Boilerplate, including a responsive fixed grid
* [skeleton-sass](https://github.com/atomicpages/skeleton-sass) - SASS port of Skeleton, includes CSS classes, but not mixins
* [Skeleton-SASS](https://github.com/lazerwalker/Skeleton-SASS) - SASS port of Skeleton, includes mixins, but not CSS classes
* with a some inspiration from [Profound Grid](http://www.profoundgrid.com/)

###TODO:
* include the option to have different gutter and margin widths, which Skeleton does not. (maybe)
* make it so i can use includes in css instead of marking up the HTML

##files
there are very few of them. poke around. it's pretty straightforward. you might want to make adjustments to __includes/skeleton/_variables.scss__.

##development

there are many ways to compile [SCSS](http://sass-lang.com/). i normally use [Compass](http://compass-style.org/), but since this project is not dependent on any of the compass features, during development, i compile with the __sass__ utility by running:
```
$ sass --watch scss/your-app.scss:stylesheets/your-app.css
```

i use [Livereload](http://livereload.com/) (on a mac) to monitor changes on the disk and refresh the browser automagically.


