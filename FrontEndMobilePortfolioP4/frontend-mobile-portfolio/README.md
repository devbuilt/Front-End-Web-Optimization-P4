##Udacity Project 4: Web Optimizing

##Summary

This project requires improving the performance of loading and rendering an existing portfolio site. The speed of the site was measured using Chrome dev tools to identify performance bottlenecks, and then optimizations were applied to address those bottlenecks.

##Steps to Launch

1. Download or clone repository.
2. Launch your favorite server to test I used node.js "http-server". Link to install (https://www.npmjs.com/package/http-server).Open terminal window and navigate to your folder directory you wish to test, and run the command: http-server and in will open port 8080.
3. Open a new terminal window and run in the same directory the command: ./ngrok http 8080.
4. You will get a public Url to test on Google PageSpeed Insights.
5. To capture the FPS in pizza.html, open developer tools in google chrome go to the timeline section and click record while scrolling.

##Optimization of views/js/css/images/pizza.html

1. Modified pizza.html by adding a style tag just above the head tag and minifying and compressing style.css and bootstrap.grid.css to prevent css render blocking and placed the sytle.css and bootstarp.grid.css link tags just above the ending body tag for page load efficiency.
2. Modified pizza.html by adding a script tag just above head tag and minifying and compressing main.js to prevent Javascript render blocking. and placed the main.js script tag just above the ending body tag for page load efficiency.
3. Modified views/images using tinyjpg.com for image compression.
4. Edited main.js line 303, 353-354 and 251-258.

##Optimization of index.html

1. Inlined with style tag in index.html link href="//fonts.googleapis.com/css?family=Open+Sans:400,700" for loading efficiency.
2. Compressed and minified style.css to prevent css render blocking.
3. Compressed and minified print.css to prevent css render blocking.
4. Moved the link and scripted tags to bottom of html page just above the body tag. This will help with loading since it will load efficiency.


## Resources

1. Google PageSpeed Insights: https://developers.google.com/speed/pagespeed/insights/
2. Image compression: https://tinyjpg.com/
3. Critical Path Css Generator: https://jonassebastianohlsson.com/
4. Css minifying: https://cssminifier.com/
5. Javascript compression: https://jscompress.com/
