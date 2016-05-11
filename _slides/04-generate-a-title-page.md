---
---

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
