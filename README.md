Precompile Ember.js templates with Handlebars 1.3.0 which supports Subexpressions, allowing for ember query query params.

Install
-------

    npm install -g ember-precompilex

Usage
-----

This module has a similar interface to the Handlebars precompiler

    ember-precompilex template... [-f OUTPUT_FILE]

If output file is omitted, the compiled template(s) will be printed to stdout.

The template's name (in the Ember.TEMPLATES object) is created by transforming
the original filename:

 1. the `.handlebars` or `.hbs` file extension is stripped
 2. any remaining `.` characters are replaced by `/` to support
    the [nested templates used by the new Ember Router][1]

[1]: http://emberjs.com/guides/routing/defining-your-routes/#toc_resources
