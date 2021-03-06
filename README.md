## Udacity: Front-End Developer(Advanced)
### P6 - Website Optimization

#### Aim
Try my best to increase the loading and response speed. Make the page rendering as soon as posible. 
1. Optimize index.html, as least 90 points to pass the PageSpeed Insights test.
2. Optimize FPS for pizza.html, reach or above 60fbs.

### What Have Been Done

#### Part 1: Optimize index.html (PageSpeed Insights)

1. Compress the image size of pizzeria.jpg (From 2.3M to 4K) 
2. Avoid using online fonts
3. Add 'media="print"' for loading print.css
4. Add 'defer' prop for loading analytics.js
5. Move <script> tag after loading analystics.js and add 'defer' prop
6. Pick some style defines out as inner css, move loading style.css to the bottom of the page

![PageSpeed Result](https://ivyfu77.github.io/p6-website-optimization/result/PageSpeed-Result.png)

#### Part 2: Optimize main.js (for 'pizza.html') (FPS)
1. For pizza background moving animation: reduce the pizzas' number, break loop when the pizza's top is higher than the screen
2. Optimize pizza resize control, avoid use Layout before reset style in a loop.
3. Compress the top image's size (From 2.4M to 139K)
4. Use getElementById or getElementByClassName to replace querySelector
5. updatePositions(): Optimize the position change loop for each 'mover'


### How to Check

#### Part 1: Optimize index.html (PageSpeed Insights)

1. Open [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) 
2. Paste the [Link](https://ivyfu77.github.io/p6-website-optimization/), click 'Analyze' to check the optimizing result.

#### Part 2: Optimize pizza.html (FPS)
1. Open the live [Link](https://ivyfu77.github.io/p6-website-optimization/views/pizza.html)
2. Use DevTools to check the FPS when scroll the screen, change the size setting.
