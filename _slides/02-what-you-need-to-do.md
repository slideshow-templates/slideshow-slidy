---
---

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
