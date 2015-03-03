# FOSS4G 2014 OpenLayers talk

OpenLayers 3 presentation for FOSS4G 2014.

## Set up

Dependencies pulled in with [npm](https://npmjs.org/).

After cloning the repo (and installing Node):

    cd talks/foss4g2014
    npm install
    npm start

Now you can view the slides by opening http://localhost:9001/ol3.html in a browser.

## OpenLayers Examples

The OpenLayers examples all share the same basic layout, so they are built from templates.  The `npm install` step above builds all examples (and more) and puts everything in the `.grunt/self` directory.  To facilitate rebuilding of examples during development, a simple server and watch task are included. This is fired up with the following:

    npm start

This will build the examples, copy over files that don't need pre-processing, start a static file server rooted in the `.grunt/self` directory, and launch a file watcher task that will re-build/copy when files change.

While this task is running, the slideshow is available at http://localhost:9001/ol3.html and examples are at http://localhost:9001/examples/.  When the slides are deployed, the examples will have the same relative path to the slides (e.g. slides can link to examples with './examples/hello-world.html').

## Credits

Credits to [reveal.js](http://lab.hakim.se/reveal-js/) for the slick presentation software, and to @tschaub for the nice npm/bower/grunt set-up.
