# Project Title
## Website Performance Optimization portfolio project by Scott Dickinson

Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed! In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

To get started, check out the repository and inspect the code.

### Getting started

To run, you can either navigate to https://culer5.github.io/Website_Optimization/, or install the project on your machine. To do that, either clone the repository using git, or click the download zip button on the right and unzip the file.

To view the optimized page, double-click index.html.

I have optimized index.html to achieve at least a 90 PageSpeed score. I've optimized the JavaScript in pizza.html to achieve a frame rate of 57  fps when scrolling. I've also reduced the time to resize pizzas in pizza.html to less than 5 ms.

#### Part 1: Optimize PageSpeed Insights score for index.html

I utilized a Chrome Extension : Critical Style Snapshot to identify the above the fold content. I inlined the critical CSS and moved the links to lower in the html file.
I utilized tinyjpg.com to compress all of my images.



#### Part 2: Optimize Frames per Second in pizza.html

To optimize views/pizza.html, you will need to modify views/js/main.js until your frames per second rate is 60 fps or lower. You will find instructive comments in main.js. 

The code review identified the following areas to correct:
 querySelectorAll is slower than getElementsByClassName, so they've been switched in main.js
 
 Move variables out of the for loops to reduce the number of times the DOM was touched so I moved that in the resize pizza function and the update positions function.
 
 In addition, I inlined the critical CSS
 
 I left off <style></style> tags in pizza.html!
 
 #### Acknowledgments:
 Learn Javascript Visually by Ivelin Demirov
 A Smarter Way to Learn Javascript by Mark Myers.
 Explore Front-End Development: Lynda.com
 
