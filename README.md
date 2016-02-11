## Website Performance Optimization portfolio project

Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed! In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).
======================================================================
-->[get started]:
----------------
download the file and run it in your favorite browser locally.

-->[page load speed]:
---------------------------------
* img compression : using ImageOptim.
* CSS/JS Minfying : all css/js files were minified to make sure faster downloading, the original files still in there, the new css/js renamed with '.min'.
* added css inline and applied to the doc. immediately better than blocking "method by Google" see references.
* alternative media CSS the print stylesheet, yes its small, its better not to be inline in HTML documents because its being used in three different pages. so as a media attribute was added just to make sure that it would only be downloaded when printing or anything related to printing.

-->[frame rate]:
----------------------------
* unnecessary JS operations were pulled out of 'for' loops, in 'views/js/main.js'.
* scroll events were changed to decouple the animations and only reflow/repaint when needed.

-->[Customization with Bootstrap]:
----------------------------------
The portfolio was built on Twitter's <a href="http://getbootstrap.com/">Bootstrap</a> framework. All custom styles are in `dist/css/portfolio.css` in the portfolio repo.

* <a href="http://getbootstrap.com/css/">Bootstrap's CSS Classes</a>
* <a href="http://getbootstrap.com/components/">Bootstrap's Components</a>

-->[Resources]:
---------------
- [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)
- [Optimize CSS Delivery](https://developers.google.com/speed/docs/insights/OptimizeCSSDelivery)
- [Leaner, Meaner, Faster Animations with requestAnimationFrame](http://www.html5rocks.com/en/tutorials/speed/animations/)
