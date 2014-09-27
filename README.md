<h2>Percentext</h2>
<h5>The jQuery plugin that adjusts font-size and letter-spacing, so you can set a percentage width for your headers.
Quick Start Guide Download on GitHub</h5>

<strong>Examples, documentation and installation guide can be found at <a href="http://www.percentext.com">Percentext.com</a>.</strong>
===========================

One of the things that I hate wasting time on is positioning and sizing headers. I can position just about everything else by specifying width or height; if I want this div to take up 50% of the width, I can just set it. 

Text is trickier. The only real metric you have to play with is font-size, and if the parent container is a flexible width (AKA the site is responsive), you can't just toy with font-size until it looks right.

I am not the first person to think of this; FitText has been around for a while, and it does a great job at tying font-size to the parent container's width. For my purposes, though, it doesn't do enough. It arbitrarily sets font-size to be 10% of the parent's width. If the container is 1000px wide, it sets the font-size to 100px. There's still quite a bit of fiddling to get it exactly right.

Percentext uses font-size and letter-spacing to ensure a perfect fit, without any fiddling. By default, it takes up 100% of the width, but it can be customized to take up a smaller percentage. For example, check out the header on <a href="http://www.percentext.com">the Percentext site</a> - The words 'Allow me to introduce' sit perfectly positioned between the 'P' and 't' of Percentext. You can resize the window, and the words stay exactly where they should. To accomplish this effect, all I did was this:

  <p>Javascript:
  <blockquote>
    
    $("#title").percentext({letterSpacing: -4});
    $("#title_caption").percentext({width: 40, letterSpacing: -2});
  </blockquote></p>

  <p>CSS:
  <blockquote>
    #title_caption {
      position: absolute;
      left: 11.7%;
    }
  </blockquote>
  

Pretty cool, right?


More examples and all the info you could possibly need are sitting over at <a href="http://www.percentext.com">Percentext.com</a>.




