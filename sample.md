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

Example:

    <?xml version="1.0" encoding="utf-8"?>
    <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
     "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
    <html xmlns="http://www.w3.org/1999/xhtml" lang="en" xml:lang="en">
    <head>
      <title>Slide Shows in XHTML</title>
      <meta name="copyright"
       content="Copyright &#169; 2005 your copyright notice" />
      <link rel="stylesheet" type="text/css" media="screen, projection, print"
       href="http://www.w3.org/Talks/Tools/Slidy2/styles/slidy.css" />
      <script src="http://www.w3.org/Talks/Tools/Slidy2/scripts/slidy.js"
       charset="utf-8" type="text/javascript"></script>
      <style type="text/css">
        <!-- your custom style rules -->
      </style>
    </head>


# Timing Your Presentation

- Sometimes it is handy to know just how much time you have to
  left to finish your presentation
- To get this feature, add the following markup to the
  content of the head element, replacing 5 by the duration
  of your presentation in minutes
      <meta name="duration" content="5" />
- The time left in minutes and seconds is shown in the footer
  next to the slide number
- The clock starts to run when you move away from the first slide
- Moving back to the first slide pauses the clock


# Generate a Title Page

If you want a separate title page with the W3C blue style, the
first slide should be as follows:

    <div class="slide cover">
     <img src="http://www.w3.org/Talks/Tools/Slidy2/graphics/keys.jpg"
      alt="Cover page images (keys)" class="cover" />
     <br clear="all" />
     <h1>HTML Slidy: Slide Shows in XHTML</h1>
     <p><a href="http://www.w3.org/People/Raggett/">Dave Raggett,</a>
     <a href="mailto:dsr@w3.org">dsr@w3.org</a></p>
    </div>

The [w3c-blue.css](http://www.w3.org/Talks/Tools/Slidy2/graphics/w3c-blue.css)
style sheet looks for the classes "slide" and "cover" on div
and img elements using the CSS selector _div.slide.cover_

This technique can be used to assign your slides to different
classes with a different appearence for each such class.

Slidy also allows you to use different background markup for
different slides, based upon shared class names, as in "foo" below.
Backgrounds without additional class names are always shown except
when the slide isn't transparent. You may need to tweak your
custom style sheet.

    <div class="background foo">
       ... background content ...
    <div>

    ...

    <div class="slide foo">
       ... slide content ...
    <div>


# Continued...

To be done
