
## Slide Show (S9) Template Pack - Slidy (W3C Blue)

The [Slidy](http://www.w3.org/Talks/Tools/#slidy) package bundled up into 
a Slide Show (S9) template pack.

Note, the package is configured to use the following headers in `slides.html.erb`:

    author: Your Name Here
    title: Your Slide Show Title Here
    copyright: Your Copyright Here

See the original [HTML Slidy: Slide Shows in XHTML](http://www.w3.org/Talks/Tools/Slidy) slides in action or
see the [Slide Show (S9) Tutorial](http://slideshow.rubyforge.org/slidy/tutorial.html)
slides generated using this template pack.
 
 
## Try It Yourself - How To Use the Template Pack

If you want to try it yourself, install (fetch) the new template pack. Issue the command:

    $ slideshow -f http://github.com/geraldb/slideshow-slidy/raw/master/slidy.txt

To check if the new template got installed, use the `-l/--list` switch/command:

    $ slideshow -l

Listing something like:

    Installed templates include:
       slidy.txt (/home/gerald/.slideshow/templates/slidy/slidy.txt)

Now you're ready to use it using the `-t/--template` switch. Example:

    $ slideshow -t slidy.txt tutorial

That's it. 



## Troubleshooting 

Trouble downloading? Do you have a direct internet connection? If not, configure your proxy using
the `HTTP_PROXY` environment variable. Sample:

    HTTP_PROXY=http://234.445.454:4341

Or with user credentials (that is, login and password):

    HTTP_PROXY=http://gerald:topsecret@234.445.454:4341

If all fails, you can always download the template pack on your own (using lets say `git` itself)
and than move the souces into your templates folder (that is, `~/.slideshow/templates`).

## Questions? Comments?

Questions? Comments?
Send them along to the [Free Web Slide Show Alternatives (S5, S6, S9, Slidy And Friends) Forum/Mailing List](http://groups.google.com/group/webslideshow).
Thanks!