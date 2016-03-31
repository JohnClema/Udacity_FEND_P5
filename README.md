## Frontend Nanodegree Mobile Portfolio
Find the non optimized versions here:

And the optimized ones here:

## How to run it
Ensure you have node.js installed with npm

Go into the root project folder and run npm install

You can run the project by

`gulp psi` will run the project present it to an ngrok url and run pagespeed insights on it for desktop and mobile.

You can also view it on github pages [here at johnclema.github.io/frontend-nanodegree-mobile-portfolio](johnclema.github.io/frontend-nanodegree-mobile-portfolio)

## Optimisations to get pizza.html to 60fps
Steps taken

1. Used gulp-image-resize to resize pizza.png to pizza-small.png
2. Changed all instances of querySelector() to getElementById() and all instances of querySelectorAll() to getElementsByClassName()
3. Moved function calls mentioned in 2. outside of loops where possible
4. Move computation of new pizza size outside loop, basing the size on the first pizza only
5. Reduced the number of pizzas being rendered to 20
6. Added backface-visibility to the css
7. Moved phase variable out of the loop and kept it to five constant
* values in an array
8. Minified main.js
