## Udacity: Front-End Developer(Advanced)
### P6 - Website Optimization

#### Aim
Try my best to increase the loading and response speed. Make the page rendering as soon as posible. 
1. Optimize index.html, as least 90 points to pass the PageSpeed Insights test.
2. Optimize FPS for pizza.html, reach or above 60fbs.

### What Have Been Done

####Part 1: Optimize index.html (PageSpeed Insights)

1. Compress the image size of pizzeria.jpg (From 2.3M to 4K) 
2. Avoid using online fonts
3. Add 'media="print"' for loading print.css
4. Add 'async' prop for loading analytics.js
5. Pick some style defines out as inner css, move loading style.css to the bottom of the page

![PageSpeed Result](https://ivyfu77.github.io/p6-website-optimization/result/PageSpeed-Result.png)

####Part 2: Optimize pizza.html (FPS)
1. Delete unnecessary and expensive 'moving pizzas' background when scroll the screen, change to fixed position background
2. Optimize pizza resize control, avoid use Layout before reset style in a loop.
3. Compress the top image's size (From 2.4M to 139K)
