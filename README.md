# Slidy (W3C Blue, Blank) - Slide Show (S9) Template Pack

## Live Preview

See [`slides.blank.html`](http://slideshow-templates.github.io/slideshow-slidy/slides.blank.html)
and [`slides.w3c.html`](http://slideshow-templates.github.io/slideshow-slidy/slides.w3c.html).


## What's Slide Show (S9)?

A Ruby gem that lets you create slide shows and author slides in plain text
using a wiki-style markup language that's easy-to-write and easy-to-read.
More [Slide Show (S9) Project Site »](http://slideshow-s9.github.io)

## Intro

The [Slidy](http://www.w3.org/Talks/Tools/Slidy2) package by Dave Raggett
bundled up into
a Slide Show (S9) template pack lets you author your slides
in a wiki-style markup language (that is, Markdown or Textile) plus
lets you use text filters and helpers for adding comments, macros,
includes, syntax highlighters and much more.

Note, the Slidy template pack is configured to use the following headers in `slides.html.erb`:

    author: Your Name Here
    title: Your Slide Show Title Here
    copyright: Your Copyright Here



## Try It Yourself - How To Use the Slidy Template Pack

If you want to try it yourself, install (fetch) the new template pack. Issue the command:

    $ slideshow install slidy

Or as an alternative clone the template pack using `git`. Issue the commands:

    $ cd ~/.slideshow/templates
    $ git clone https://github.com/slideshow-templates/slideshow-slidy.git

To check if the new template got installed, use the `list` command:

    $ slideshow list

Listing something like:

    Installed template packs include:
       slidy (~/.slideshow/templates/slidy/slidy.txt)

Tip: To get started use the included quick starter sample. Issue the command:

    $ slideshow new -t slidy

Now you will have a copy of the Slidy Quick Starter sample
(that is, [`slidy.text`](https://raw.github.com/slideshow-templates/slideshow-slidy/gh-pages/sample.md))
in Markdown in your working folder.

```
title: HTML Slidy: Slide Shows in HTML and XHTML
author: Dave Raggett
copyright: Copyright © 2005-2010 W3C (MIT, ERCIM, Keio)


# Slide Shows in HTML and XHTML

- You can now create accessible slide shows with ease
- Works across browsers and is operated like PowerPoint
  - Advance to next slide with mouse click, space bar or swipe right
  - Move forward/backward between slides with Cursor Left,
    Cursor Right, __Pg Up__ and __Pg Dn__ keys, or swipe right or left
  - __Home__ key for first slide, __End__ key for last slide
  - "__C__" key for an automatically generated
    table of contents, or click on "contents" on the toolbar or
    swipe up or down
  - Function __F11__ to go full screen and back
  - The "__F__" key toggles the display of the footer
  - The "__A__" key toggles display of current vs all slides
    - Try it now to see how to include notes for handouts (this is
      explained in the notes following this slide)
  - Font sizes automatically adapt to browser window size
    - __S__ and __B__ keys for manual control (or < and >, or the __-__ and
      __+__ keys on the number pad
    - Use CSS to set a relative font size on a given slide to make
      the content bigger or smaller than on other slides
  - Switching off JavaScript reveals all slides
- _Now move to next slide to see how it works_


# What you need to do

- Each presentation is a single XHTML file
- Each slide is enclosed in `<div class='slide'> ... </div>`
  - The `div` element will be created automatically for `h1`
    elements that are direct children of the body element.
- Use regular markup within each slide
- The document head includes two links:
  - The slide show style sheet:
    [http://www.w3.org/Talks/Tools/Slidy2/styles/slidy.css](http://www.w3.org/Talks/Tools/Slidy2/styles/slidy.css)
  - The slide show script:
    [http://www.w3.org/Talks/Tools/Slidy2/scripts/slidy.js](http://www.w3.org/Talks/Tools/Slidy2/scripts/slidy.js)
  - Or you can link to the compressed version of the script which is about
    one seventh the size, see
    [http://www.w3.org/Talks/Tools/Slidy2/scripts/slidy.js.gz](http://www.w3.org/Talks/Tools/Slidy2/scripts/slidy.js.gz)
  - If you are using XHTML, remember to use `</script>` and `</style>`
    as per [Appendix C.3](http://www.w3.org/TR/xhtml1/#C_3)
```


Showtime! Let's use the `-t/--template` switch to build the
sample slide show. Example:

    $ slideshow build slidy.text -t slidy

Open up the generated `slidy.html` page in your browser. Voila. That's it.

Bonus: Open up the generated `slidy.w3c.html` page
to see the W3C Blue theme in action in your browser.

## Questions? Comments?

Questions? Comments?
Send them along to the [wwwmake forum/mailing list](http://groups.google.com/group/wwwmake).
Thanks!
