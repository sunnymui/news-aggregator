# Web Performance Optimized News Agreggator App

I fixed multiple performance issues with this web application to help it reach an acceptable fps. I refactored to avoid layout thrashing, slimmed some heavy CSS styles, refactored code to replace unnecessarily heavy JS calculations with CSS solutions, replaced effects requiring layout with ones that only use the compositor (where possible), promoted some layers + removed unnecessarily promoted layers, switched setInterval loops to requestAnimationFrame, refactored to avoid unnecessary DOM appends, implemented some node clearing/event listener removals to preserve memory, and fixed some touch bugs.

# Below are the original project requirements

**Please note: this code is intended for you to hone your debugging skills. It contains a lot of code that you should not use in production!**

This is a simple web app that shows the top stories from [Hacker News](https://news.ycombinator.com/news) via [its API](http://blog.ycombinator.com/hacker-news-api).

Unfortunately it has a bunch of performance issues, such as:

* Layout Thrashing
* Expensive painting
* Unnecessary layouts
* Long-running and badly-timed JavaScript
* Bad touch handling

Your mission is to find and fix the issues, and make the app gloriously performant!

## License

See /LICENSE for more.

This is not a Google product.
